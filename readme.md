 
 '''
	import matplotlib.pyplot as plt
	plt.rcParams['figure.figsize'] = [10, 5]

	import numpy as np; np.random.seed(sum(map(ord, 'calmap')))
	import pandas as pd
	import calmap

	all_days = pd.date_range('1/15/2014', periods=700, freq='D')
	days = np.random.choice(all_days, 500)
	events = pd.Series(np.random.randn(len(days)), index=days)

	plt.rcParams['figure.figsize'] = [20, 5]

	import warnings
	warnings.filterwarnings('ignore')
	calmap.yearplot(events, year=2015)
 '''