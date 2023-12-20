# How to load multiple .NET MAUI SfDataGrid to a Layout

You can to load multiple SfDataGrid’s in single view based on the requirement. In the below code multiple SfDataGrid has been loaded inside Grid layout and defined using RowDefinition.

## XAML
```XML
<Grid RowDefinitions="*,*">

    <syncfusion:SfDataGrid  Grid.Row="0"
                        ItemsSource="{Binding Employees}"
                        AutoGenerateColumnsMode="None"
                        DefaultColumnWidth="155">
        <syncfusion:SfDataGrid.Columns>
            <syncfusion:DataGridTextColumn MappingName="EmployeeID"
                                        HeaderText="Employee ID" />
            <syncfusion:DataGridTextColumn MappingName="Name"
                                        HeaderText="Name" />
            <syncfusion:DataGridTextColumn MappingName="IDNumber"
                            HeaderText="ID Number" />
        </syncfusion:SfDataGrid.Columns>
    </syncfusion:SfDataGrid>

    <syncfusion:SfDataGrid  Grid.Row="1"
                        ItemsSource="{Binding Employees}"
                        AutoGenerateColumnsMode="None"
                        DefaultColumnWidth="155">
        <syncfusion:SfDataGrid.Columns>
            <syncfusion:DataGridTextColumn MappingName="EmployeeID"
                                        HeaderText="Employee ID" />
            <syncfusion:DataGridTextColumn MappingName="Name"
                                        HeaderText="Name" />
            <syncfusion:DataGridTextColumn MappingName="IDNumber"
                            HeaderText="ID Number" />
        </syncfusion:SfDataGrid.Columns>
    </syncfusion:SfDataGrid>

</Grid>

```

The following screenshot shows  Multiple DataGrid in a single Layout.

![Multiple DataGrid in single layout](Multiple_DataGrid_SingleLayout.png)

[View sample in GitHub](https://github.com/SyncfusionExamples/How-to-load-multiple-.NET-MAUI-SfDataGrid-s-to-a-layout/tree/master)

Take a moment to pursue this [documentation](https://help.syncfusion.com/maui/datagrid/overview), where you can find more about Syncfusion .NET MAUI DataGrid (SfDataGrid) with code examples.
Please refer to this [link](https://www.syncfusion.com/maui-controls/maui-datagrid) to learn about the essential features of Syncfusion .NET MAUI DataGrid(SfDataGrid).

### Conclusion
I hope you enjoyed learning about how to show multiple DataGrid in a single layout.

You can refer to our [.NET MAUI DataGrid's feature tour](https://www.syncfusion.com/maui-controls/maui-datagrid) page to know about its other groundbreaking feature representations. You can also explore our .NET MAUI DataGrid Documentation to understand how to present and manipulate data.
For current customers, you can check out our .NET MAUI components from the [License and Downloads](https://www.syncfusion.com/account/downloads) page. If you are new to Syncfusion, you can try our 30-day free trial to check out our .NET MAUI DataGrid and other .NET MAUI components.
If you have any queries or require clarifications, please let us know in comments below. You can also contact us through our [support forums](https://www.syncfusion.com/forums), [Direct-Trac](https://support.syncfusion.com/account/login?ReturnUrl=%2Faccount%2Fconnect%2Fauthorize%2Fcallback%3Fclient_id%3Dc54e52f3eb3cde0c3f20474f1bc179ed%26redirect_uri%3Dhttps%253A%252F%252Fsupport.syncfusion.com%252Fagent%252Flogincallback%26response_type%3Dcode%26scope%3Dopenid%2520profile%2520agent.api%2520integration.api%2520offline_access%2520kb.api%26state%3D8db41f98953a4d9ba40407b150ad4cf2%26code_challenge%3DvwHoT64z2h21eP_A9g7JWtr3vp3iPrvSjfh5hN5C7IE%26code_challenge_method%3DS256%26response_mode%3Dquery) or [feedback portal](https://www.syncfusion.com/feedback/maui?control=sfdatagrid). We are always happy to assist you!