//how to use
//inject depency in dataSearch.module.js:
	var moduleDependencies = ['atmira.ui.tabletree']
//inject in view.html <atmira-ui-tabletree tree-data="dataSearchCtrl.tree_data"></atmira-ui-tabletree>
//inject <script src="./bower_components/atmira-ui-tabletree/dist/tabletree.js"></script> into index.html 
//inject <link rel="stylesheet" href="./bower_components/atmira-ui-tabletree/dist/tabletree.css"> into index.html
// create an array in dataSearch.component.js:
     vm.tree_data = [
      {Name:"USA",Area:9826675,Population:318212000,TimeZone:"UTC -5 to -10",
      children:[
        {Name:"California", Area:423970,Population:38340000,TimeZone:"Pacific Time"},
        {Name:"Illinois", Area:57914,Population:12882135,TimeZone:"Central Time Zone"}
      ]
      },
        {Name:"Texas",Area:268581,Population:26448193,TimeZone:"Mountain",
          children:[
          {Name:"Illinois", Area:57914,Population:12882135,TimeZone:"Central Time Zone"}
        ]
      }
      ];