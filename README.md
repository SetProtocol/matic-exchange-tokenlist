Obtained by running this command:
  const url = 'https://api.thegraph.com/subgraphs/name/sushiswap/matic-exchange';
  const properties = ['id', 'symbol', 'name', 'decimals', 'volumeUSD'];

  const response = await pageResults({
    api: url,
    query: {
      entity: 'tokens',
      properties: properties,
    },
  });