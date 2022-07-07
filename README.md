option = {
    tooltip: {
        trigger: 'item',
        triggerOn: 'mousemove'
    },
    series: {
        type: 'sankey',
        bottom: '10%',
        emphasis: {
            focus: 'adjacency'
        },
        data: [ {
            name: '清洁能源',
            'itemStyle':{
                'color':'#ffecd2',
            }
        }, {
            name: '多种用途',
            'itemStyle':{
                'color':'#f7f7c3',
            }
        }, {
            name: '清洁交通',
            'itemStyle':{
                'color':'#E8B4',
            }
        }, {
            name: '生态保护和适应气候变化',
            'itemStyle':{
                'color':'#fde998',
            }
        },{
            name: '地方政府债',
            'itemStyle':{
                'color':'#c1d8ac',
            }
        },{
            name: '公司债',
            'itemStyle':{
                'color':'#fcf1A4',
            }
        },{
            name: '污染防治',
            'itemStyle':{
                'color':'#F9C0AF',
            }
        }
        ,{
            name: '短期融资券',
            'itemStyle':{
                'color':'#F9C0AF',
            }
        },{
            name: '中期票据',
            'itemStyle':{
                'color':'#f9e5e8',
            }
        }
        ],
        links: [
             
                {source: '中期票据', target: '清洁交通', value: 1},
                {source: '中期票据', target: '清洁能源', value: 4},
                {source: '金融债', target: '多种用途', value: 1},
                {source: '公司债', target: '清洁能源', value: 1},
                {source: '公司债', target: '多种用途', value: 1},
                {source: '短期融资券', target: '清洁能源', value: 1},
                {source: '地方政府债', target: '污染防治', value: 1},
                {source: '地方政府债', target: '清洁交通', value: 3},
                {source: '地方政府债', target: '生态保护和适应气候变化', value: 2},
                {source: '地方政府债', target: '多种用途', value: 2},
            ],
            label: {
                position: 'top'
            },
            lineStyle: {
                color: 'gradient',
                curveness: 0.6
            }
        }
};

