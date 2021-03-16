<template lang="pug">
	.svgResponsive(ref="field" @resize="reSize")
		chart(:points="data" tky="5")
</template>

<script>
// @ is an alias to /src
import WeDoChart from "we-do-chart";
import "we-do-chart/we-do-chart.min.css";
/* eslint-disable */
export default {
	name: "Home",
	components: {
		'chart':WeDoChart
	},
  data: () => ({
	data: [{name:'sto',data:[
			{tm:'2019-12-07',price:148.77},
			{tm:'2019-12-08',price:151.26},
			{tm:'2019-12-09',price:148.23},
			{tm:'2019-12-10',price:146.27},
			{tm:'2019-12-11',price:143.61},
			{tm:'2019-12-12',price:145.60},
			{tm:'2019-12-13',price:144.94},
			{tm:'2019-12-14',price:142.87},
			{tm:'2019-12-15',price:143.11},
			{tm:'2019-12-16',price:133.61},
			{tm:'2019-12-17',price:122.60},
			{tm:'2019-12-18',price:133.09},
			{tm:'2019-12-19',price:129.32},
			{tm:'2019-12-20',price:129.07},
			{tm:'2019-12-21',price:128.13},
			{tm:'2019-12-22',price:132.37},
			{tm:'2019-12-23',price:128.61},
			{tm:'2019-12-24',price:129.06},
			{tm:'2019-12-25',price:126.45},
			{tm:'2019-12-26',price:126.36},
			{tm:'2019-12-27',price:127.21},
			{tm:'2019-12-28',price:128.32},
			{tm:'2019-12-29',price:134.76},
			{tm:'2019-12-30',price:132.63},
			{tm:'2019-12-31',price:129.61},
			{tm:'2020-01-01',price:130.80},
			{tm:'2020-01-02',price:127.41},
			{tm:'2020-01-03',price:134.17},
			{tm:'2020-01-04',price:135.07},
			{tm:'2020-01-05',price:136.28},
			{tm:'2020-01-06',price:144.30},
			{tm:'2020-01-07',price:143.54},
			{tm:'2020-01-08',price:141.26},
			{tm:'2020-01-09',price:138.98},
			{tm:'2020-01-10',price:143.96},
			{tm:'2020-01-11',price:142.93},
			{tm:'2020-01-12',price:145.87},
			{tm:'2020-01-13',price:144.23},
			{tm:'2020-01-14',price:165.96},
			{tm:'2020-01-15',price:166.23},
			{tm:'2020-01-16',price:164.39},
			{tm:'2020-01-17',price:170.78},
			{tm:'2020-01-18',price:175.37},
			{tm:'2020-01-19',price:166.97},
			{tm:'2020-01-20',price:167.12},
			{tm:'2020-01-21',price:169.70},
			{tm:'2020-01-22',price:168.29},
			{tm:'2020-01-23',price:162.93},
			{tm:'2020-01-24',price:163.05},
			{tm:'2020-01-25',price:161.28},
			{tm:'2020-01-26',price:168.08},
			{tm:'2020-01-27',price:170.93},
			{tm:'2020-01-28',price:176.37},
			{tm:'2020-01-29',price:175.05},
			{tm:'2020-01-30',price:184.69},
			{tm:'2020-01-31',price:180.16},
			{tm:'2020-02-01',price:183.67},
			{tm:'2020-02-02',price:188.62},
			{tm:'2020-02-03',price:189.87},
			{tm:'2020-02-04',price:189.25},
			{tm:'2020-02-05',price:204.23},
			{tm:'2020-02-06',price:212.34},
			{tm:'2020-02-07',price:222.73},
			{tm:'2020-02-08',price:223.15},
			{tm:'2020-02-09',price:228.58},
			{tm:'2020-02-10',price:223.52},
			{tm:'2020-02-11',price:235.85},
			{tm:'2020-02-12',price:265.41},
			{tm:'2020-02-13',price:268.10},
			{tm:'2020-02-14',price:284.22},
			{tm:'2020-02-15',price:264.73},
			{tm:'2020-02-16',price:259.89},
			{tm:'2020-02-17',price:266.36},
			{tm:'2020-02-18',price:281.94},
			{tm:'2020-02-19',price:259.76},
			{tm:'2020-02-20',price:257.95},
			{tm:'2020-02-21',price:265.60},
			{tm:'2020-02-22',price:262.33},
			{tm:'2020-02-23',price:273.75},
			{tm:'2020-02-24',price:265.22},
			{tm:'2020-02-25',price:247.82},
			{tm:'2020-02-26',price:225.68},
			{tm:'2020-02-27',price:226.75},
			{tm:'2020-02-28',price:226.76},
			{tm:'2020-02-29',price:219.85},
			{tm:'2020-03-01',price:218.97},
			{tm:'2020-03-02',price:230.57},
			{tm:'2020-03-03',price:224.48},
			{tm:'2020-03-04',price:224.52},
			{tm:'2020-03-05',price:229.27},
			{tm:'2020-03-06',price:243.53},
			{tm:'2020-03-07',price:237.85},
			{tm:'2020-03-08',price:200.69},
			{tm:'2020-03-09',price:201.99},
			{tm:'2020-03-10',price:200.77},
			{tm:'2020-03-11',price:194.87},
			{tm:'2020-03-12',price:112.35},
			{tm:'2020-03-13',price:133.20},
			{tm:'2020-03-14',price:123.31},
			{tm:'2020-03-15',price:125.21},]}
	]
  }),
  mounted() {
		window.addEventListener("resize", this.reSize);
	},
	methods:{
		reSize(e) {
			console.log(" reSize ",e);
			
		}
	}
};
</script>
<style lang='stylus'>
.svgResponsive {
		  width: 500px; height: 500px; background-color: snow; resize: both ;
		  padding-right  30px
		  padding-top 1px
		  border: 2px solid; overflow: auto;
	}
.cbox
	width 500px
	height 500px
	background-color azure
	text-align center
	margin auto
.leftThumb
	fill red
.chartSheet
		stroke transparent		
</style>
