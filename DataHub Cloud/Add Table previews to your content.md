# Adding a Table Component

Datahub Cloud allows you to easily add table components to your datasets or data stories. Here’s how you can do it using different approaches:

## FlatUiTable

The `FlatUiTable` component dynamically renders your dataset (whether it’s an array of objects, a CSV file, inline CSV, or an external source) in a table view. It offers features like filtering, sorting, pagination, and export options.

### Adding Data from Array Objects

To display static data in your story, pass a `data.values` attribute to the component in your `.md` file. For example:

```js
<FlatUiTable
  data={{
    values: [
      { FirstName: "Jon", LastName: "Snow", Age: 35 },
      { FirstName: "Cersei", LastName: "Lannister", Age: 42 },
      { FirstName: "Jaime", LastName: "Lannister", Age: 45 },
    ],
  }}
/>
```

To visualize and interact with your data:

<FlatUiTable
data={{
    values: [
      {
        FirstName: "Jon",
        LastName: "Snow",
        Age: 35,
      },
      {
        FirstName: "Cersei",
        LastName: "Lannister",
        Age: 42,
      },
      {
        FirstName: "Jaime",
        LastName: "Lannister",
        Age: 45,
      }
    ]
  }}
/>

### Adding Data from External Sources

Your data source could be a csv in you githup project or even an external CSV file. You can display it by passing the `data.url` property to the `FlatUiTable` component:

```js
<FlatUiTable
  data={{
    url: "/assets/data.csv",
  }}
/>
```

And the table will be rendered like this:

<FlatUiTable
data={{
    url: "/assets/data.csv",
  }}
/>

### Using Inline CSV

You can also write inline CSV data using the `data.csv` property:

```js
<FlatUiTable
  data={{
    csv: `
    Year,Temp Anomaly
    1850,-0.418
    2020,0.923
    `,
  }}
/>
```

To see it in action:

<FlatUiTable
data={{
    csv: `
    Year,Temp Anomaly
    1850,-0.418
    2020,0.923
    `,
  }}
/>

## Excel

If you’re working with Excel files, the `Excel` component is a great option to display your data. This component supports features like filtering, sorting, and viewing multiple sheets, making it easy to interact with your Excel data directly in your story.

```js
<Excel
  data={{
    url: "https://storage.portaljs.org/IC-Gantt-Chart-Project-Template-8857.xlsx",
    //you can also use local csv and xlsx files
  }}
/>
```

<Excel
data={{
    url: "https://storage.portaljs.org/IC-Gantt-Chart-Project-Template-8857.xlsx",
  }}
/>
