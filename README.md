cube(`DwsMemberTagDetail`, {
  sql: `SELECT * FROM clickhouse_test.dws_member_tag_detail`,
  
  preAggregations: {
    // Pre-Aggregations definitions go here
    // Learn more here: https://cube.dev/docs/caching/pre-aggregations/getting-started
  },
  
  joins: {
    
  },
  
  measures: {
    count: {
      type: `count`,
      drillMembers: []
    }
  },
  
  dimensions: {
    userId: {
      sql: `user_id`,
      type: `number`
    },
    
    paidPriceSum1d: {
      sql: `paid_price_sum_1d`,
      type: `number`,
      title: `Paid Price Sum 1d`
    },
    
    paidPriceSum3d: {
      sql: `paid_price_sum_3d`,
      type: `number`,
      title: `Paid Price Sum 3d`
    },
    
    paidPriceSum7d: {
      sql: `paid_price_sum_7d`,
      type: `number`,
      title: `Paid Price Sum 7d`
    },
    
    paidPriceSum15d: {
      sql: `paid_price_sum_15d`,
      type: `number`,
      title: `Paid Price Sum 15d`
    },
    
    paidPriceSum30d: {
      sql: `paid_price_sum_30d`,
      type: `number`,
      title: `Paid Price Sum 30d`
    },
    
    paidPriceSum60d: {
      sql: `paid_price_sum_60d`,
      type: `number`,
      title: `Paid Price Sum 60d`
    },
    
    paidPriceSum90d: {
      sql: `paid_price_sum_90d`,
      type: `number`,
      title: `Paid Price Sum 90d`
    },
    
    paidPriceSum180d: {
      sql: `paid_price_sum_180d`,
      type: `number`,
      title: `Paid Price Sum 180d`
    },
    
    paidPriceCount1d: {
      sql: `paid_price_count_1d`,
      type: `number`,
      title: `Paid Price Count 1d`
    },
    
    paidPriceCount3d: {
      sql: `paid_price_count_3d`,
      type: `number`,
      title: `Paid Price Count 3d`
    },
    
    paidPriceCount7d: {
      sql: `paid_price_count_7d`,
      type: `number`,
      title: `Paid Price Count 7d`
    },
    
    paidPriceCount15d: {
      sql: `paid_price_count_15d`,
      type: `number`,
      title: `Paid Price Count 15d`
    },
    
    paidPriceCount30d: {
      sql: `paid_price_count_30d`,
      type: `number`,
      title: `Paid Price Count 30d`
    },
    
    paidPriceCount60d: {
      sql: `paid_price_count_60d`,
      type: `number`,
      title: `Paid Price Count 60d`
    },
    
    paidPriceCount90d: {
      sql: `paid_price_count_90d`,
      type: `number`,
      title: `Paid Price Count 90d`
    },
    
    paidPriceCount180d: {
      sql: `paid_price_count_180d`,
      type: `number`,
      title: `Paid Price Count 180d`
    },
    
    paidPriceAvg1d: {
      sql: `paid_price_avg_1d`,
      type: `number`,
      title: `Paid Price Avg 1d`
    },
    
    paidPriceAvg3d: {
      sql: `paid_price_avg_3d`,
      type: `number`,
      title: `Paid Price Avg 3d`
    },
    
    paidPriceAvg7d: {
      sql: `paid_price_avg_7d`,
      type: `number`,
      title: `Paid Price Avg 7d`
    },
    
    paidPriceAvg15d: {
      sql: `paid_price_avg_15d`,
      type: `number`,
      title: `Paid Price Avg 15d`
    },
    
    paidPriceAvg30d: {
      sql: `paid_price_avg_30d`,
      type: `number`,
      title: `Paid Price Avg 30d`
    },
    
    paidPriceAvg60d: {
      sql: `paid_price_avg_60d`,
      type: `number`,
      title: `Paid Price Avg 60d`
    },
    
    paidPriceAvg90d: {
      sql: `paid_price_avg_90d`,
      type: `number`,
      title: `Paid Price Avg 90d`
    },
    
    paidPriceAvg180d: {
      sql: `paid_price_avg_180d`,
      type: `number`,
      title: `Paid Price Avg 180d`
    },
    
    vipLevel: {
      sql: `vip_level`,
      type: `string`
    },
    
    store1d: {
      sql: `store_1d`,
      type: `string`,
      title: `Store 1d`
    },
    
    store3d: {
      sql: `store_3d`,
      type: `string`,
      title: `Store 3d`
    },
    
    store7d: {
      sql: `store_7d`,
      type: `string`,
      title: `Store 7d`
    },
    
    store15d: {
      sql: `store_15d`,
      type: `string`,
      title: `Store 15d`
    },
    
    store30d: {
      sql: `store_30d`,
      type: `string`,
      title: `Store 30d`
    },
    
    store60d: {
      sql: `store_60d`,
      type: `string`,
      title: `Store 60d`
    },
    
    store90d: {
      sql: `store_90d`,
      type: `string`,
      title: `Store 90d`
    },
    
    store180d: {
      sql: `store_180d`,
      type: `string`,
      title: `Store 180d`
    },
    
    ds: {
      sql: `ds`,
      type: `time`,
      primaryKey: true
    },
    
    lastOrderDay: {
      sql: `last_order_day`,
      type: `time`
    },
    
    firstOrderDay: {
      sql: `first_order_day`,
      type: `time`
    }
  }
});
