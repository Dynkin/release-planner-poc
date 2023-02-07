<template>
  <JSCharting :options="chartOptions" class="columnChart"></JSCharting>
</template>

<script>
import JSCharting from "jscharting-vue";

export default {
  name: "ExampleChart",
  data() {
    return {
      chartOptions: {
        type: "column",
        yAxis: {
          scale_type: "stacked",
          label_text: "Story Points",
        },
        title_label_text: "Релизы",
        xAxis: {
          scale_type: "time",
          label_text: "Date",
        },
        series: [
          {
            name: "Release 45.1.0",
            id: "s1",
            points: [
              {
                x: "1/1/2023",
                y: 230,
              },
              {
                x: "1/1/2023",
                y: 240,
              },
              {
                x: "1/1/2023",
                y: 267,
              },
              {
                x: "1/1/2023",
                y: 238,
              },
            ],
          },
          {
            name: "Release 45.2.0",
            id: "s2",
            points: [
              {
                x: "2/1/2023",
                y: 325,
              },
              {
                x: "2/1/2023",
                y: 367,
              },
              {
                x: "2/1/2023",
                y: 382,
              },
              {
                x: "2/1/2023",
                y: 371,
              },
            ],
          },
          {
            name: "Release 46.0.0",
            id: "s3",
            points: [
              {
                x: "3/1/2023",
                y: 285,
              },
              {
                x: "3/1/2023",
                y: 292,
              },
              {
                x: "3/1/2023",
                y: 267,
              },
              {
                x: "3/1/2023",
                y: 218,
              },
            ],
          },
        ],
      },
    };
  },
  components: {
    JSCharting,
  },
};
</script>

<style>
.columnChart {
  height: 300px;
}
</style>s