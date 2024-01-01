annotation-target::[[Books/Data Science from Scratch.pdf]]

>%%
>```annotation-json
>{"created":"2022-11-02T17:51:32.718Z","text":"Add function for Vectorwritten in python","updated":"2022-11-02T17:51:32.718Z","document":{"title":"Data Science from Scratch","link":[{"href":"urn:x-pdf:075b70806d7268e551e501c8259b56a7"},{"href":"vault:/Books/Data Science from Scratch.pdf"}],"documentFingerprint":"075b70806d7268e551e501c8259b56a7"},"uri":"vault:/Books/Data Science from Scratch.pdf","target":[{"source":"vault:/Books/Data Science from Scratch.pdf","selector":[{"type":"TextPositionSelector","start":118134,"end":118251},{"type":"TextQuoteSelector","exact":"def vector_add(v, w):    \"\"\"adds corresponding elements\"\"\"    return [v_i + w_i            for v_i, w_i in zip(v, w)]","prefix":" add the corresponding elements:","suffix":"50 | Chapter 4: Linear Algebraww"}]}]}
>```
>%%
>*%%PREFIX%%add the corresponding elements:%%HIGHLIGHT%% ==def vector_add(v, w):    """adds corresponding elements"""    return [v_i + w_i            for v_i, w_i in zip(v, w)]== %%POSTFIX%%50 | Chapter 4: Linear Algebraww*
>%%LINK%%[[#^yuckctdemk|show annotation]]
>%%COMMENT%%
>Add function for Vectorwritten in python
>%%TAGS%%
>
^yuckctdemk


>%%
>```annotation-json
>{"created":"2022-11-02T18:03:28.693Z","text":"Use of `reduce` and `partial`.","updated":"2022-11-02T18:03:28.693Z","document":{"title":"Data Science from Scratch","link":[{"href":"urn:x-pdf:075b70806d7268e551e501c8259b56a7"},{"href":"vault:/Books/Data Science from Scratch.pdf"}],"documentFingerprint":"075b70806d7268e551e501c8259b56a7"},"uri":"vault:/Books/Data Science from Scratch.pdf","target":[{"source":"vault:/Books/Data Science from Scratch.pdf","selector":[{"type":"TextPositionSelector","start":119280,"end":119390},{"type":"TextQuoteSelector","exact":"def vector_sum(vectors):    return reduce(vector_add, vectors)or even:vector_sum = partial(reduce, vector_add)","prefix":"ly using higher-order functions:","suffix":"although this last one is probab"}]}]}
>```
>%%
>*%%PREFIX%%ly using higher-order functions:%%HIGHLIGHT%% ==def vector_sum(vectors):    return reduce(vector_add, vectors)or even:vector_sum = partial(reduce, vector_add)== %%POSTFIX%%although this last one is probab*
>%%LINK%%[[#^7rrz4g8l4hc|show annotation]]
>%%COMMENT%%
>Use of `reduce` and `partial`.
>%%TAGS%%
>
^7rrz4g8l4hc


>%%
>```annotation-json
>{"created":"2022-11-02T18:06:29.205Z","text":"Dot product of vectors","updated":"2022-11-02T18:06:29.205Z","document":{"title":"Data Science from Scratch","link":[{"href":"urn:x-pdf:075b70806d7268e551e501c8259b56a7"},{"href":"vault:/Books/Data Science from Scratch.pdf"}],"documentFingerprint":"075b70806d7268e551e501c8259b56a7"},"uri":"vault:/Books/Data Science from Scratch.pdf","target":[{"source":"vault:/Books/Data Science from Scratch.pdf","selector":[{"type":"TextPositionSelector","start":120098,"end":120214},{"type":"TextQuoteSelector","exact":"def dot(v, w):    \"\"\"v_1 * w_1 + ... + v_n * w_n\"\"\"    return sum(v_i * w_i               for v_i, w_i in zip(v, w))","prefix":" oftheir componentwise products:","suffix":"Vectors | 51www.it-ebooks.infoTh"}]}]}
>```
>%%
>*%%PREFIX%%oftheir componentwise products:%%HIGHLIGHT%% ==def dot(v, w):    """v_1 * w_1 + ... + v_n * w_n"""    return sum(v_i * w_i               for v_i, w_i in zip(v, w))== %%POSTFIX%%Vectors | 51www.it-ebooks.infoTh*
>%%LINK%%[[#^nyb1r7sjkhn|show annotation]]
>%%COMMENT%%
>Dot product of vectors
>%%TAGS%%
>
^nyb1r7sjkhn


>%%
>```annotation-json
>{"created":"2022-11-03T09:28:28.447Z","text":"Matrix generation code with Number of columns and rows provided.","updated":"2022-11-03T09:28:28.447Z","document":{"title":"Data Science from Scratch","link":[{"href":"urn:x-pdf:075b70806d7268e551e501c8259b56a7"},{"href":"vault:/Books/Data Science from Scratch.pdf"}],"documentFingerprint":"075b70806d7268e551e501c8259b56a7"},"uri":"vault:/Books/Data Science from Scratch.pdf","target":[{"source":"vault:/Books/Data Science from Scratch.pdf","selector":[{"type":"TextPositionSelector","start":123406,"end":123737},{"type":"TextQuoteSelector","exact":"def make_matrix(num_rows, num_cols, entry_fn):    \"\"\"returns a num_rows x num_cols matrix    whose (i,j)th entry is entry_fn(i, j)\"\"\"    return [[entry_fn(i, j)             # given i, create a list             for j in range(num_cols)]  #   [entry_fn(i, 0), ... ]            for i in range(num_rows)]   # create one list for each i","prefix":"ing a nested list comprehension:","suffix":"Given this function, you could m"}]}]}
>```
>%%
>*%%PREFIX%%ing a nested list comprehension:%%HIGHLIGHT%% ==def make_matrix(num_rows, num_cols, entry_fn):    """returns a num_rows x num_cols matrix    whose (i,j)th entry is entry_fn(i, j)"""    return [[entry_fn(i, j)             # given i, create a list             for j in range(num_cols)]  #   [entry_fn(i, 0), ... ]            for i in range(num_rows)]   # create one list for each i== %%POSTFIX%%Given this function, you could m*
>%%LINK%%[[#^aogb760ugma|show annotation]]
>%%COMMENT%%
>Matrix generation code with Number of columns and rows provided.
>%%TAGS%%
>
^aogb760ugma


>%%
>```annotation-json
>{"created":"2022-11-03T10:45:34.106Z","text":"Mean of dataset and its function\n","updated":"2022-11-03T10:45:34.106Z","document":{"title":"Data Science from Scratch","link":[{"href":"urn:x-pdf:075b70806d7268e551e501c8259b56a7"},{"href":"vault:/Books/Data Science from Scratch.pdf"}],"documentFingerprint":"075b70806d7268e551e501c8259b56a7"},"uri":"vault:/Books/Data Science from Scratch.pdf","target":[{"source":"vault:/Books/Data Science from Scratch.pdf","selector":[{"type":"TextPositionSelector","start":130105,"end":130287},{"type":"TextQuoteSelector","exact":"Central TendenciesUsually, we’ll want some notion of where our data is centered. Most commonly we’lluse the mean (or average), which is just the sum of the data divided by its count:","prefix":"9But we’re only getting started.","suffix":"# this isn't right if you don't "}]}]}
>```
>%%
>*%%PREFIX%%9But we’re only getting started.%%HIGHLIGHT%% ==Central TendenciesUsually, we’ll want some notion of where our data is centered. Most commonly we’lluse the mean (or average), which is just the sum of the data divided by its count:== %%POSTFIX%%# this isn't right if you don't*
>%%LINK%%[[#^d96q5i5q8qf|show annotation]]
>%%COMMENT%%
>Mean of dataset and its function
>
>%%TAGS%%
>
^d96q5i5q8qf


>%%
>```annotation-json
>{"created":"2022-11-03T11:18:46.300Z","text":"Outliers are bad for presentations and prediction.\n","updated":"2022-11-03T11:18:46.300Z","document":{"title":"Data Science from Scratch","link":[{"href":"urn:x-pdf:075b70806d7268e551e501c8259b56a7"},{"href":"vault:/Books/Data Science from Scratch.pdf"}],"documentFingerprint":"075b70806d7268e551e501c8259b56a7"},"uri":"vault:/Books/Data Science from Scratch.pdf","target":[{"source":"vault:/Books/Data Science from Scratch.pdf","selector":[{"type":"TextPositionSelector","start":132493,"end":132890},{"type":"TextQuoteSelector","exact":"At the same time, the mean is very sensitive to outliers in our data. If our friendliestuser  had  200  friends  (instead  of  100),  then  the  mean  would  rise  to  7.82,  while  themedian would stay the same. If outliers are likely to be bad data (or otherwise unrep‐resentative of whatever phenomenon we’re trying to understand), then the mean cansometimes  give  us  a  misleading  picture. ","prefix":"ok, so we have to sort the data.","suffix":" For  example,  the  story  is  "}]}]}
>```
>%%
>*%%PREFIX%%ok, so we have to sort the data.%%HIGHLIGHT%% ==At the same time, the mean is very sensitive to outliers in our data. If our friendliestuser  had  200  friends  (instead  of  100),  then  the  mean  would  rise  to  7.82,  while  themedian would stay the same. If outliers are likely to be bad data (or otherwise unrep‐resentative of whatever phenomenon we’re trying to understand), then the mean cansometimes  give  us  a  misleading  picture.== %%POSTFIX%%For  example,  the  story  is*
>%%LINK%%[[#^7lg6p56p4ee|show annotation]]
>%%COMMENT%%
>Outliers are bad for presentations and prediction.
>
>%%TAGS%%
>
^7lg6p56p4ee


>%%
>```annotation-json
>{"created":"2022-11-03T11:19:47.064Z","text":"Quantile to filter data based on value range.","updated":"2022-11-03T11:19:47.064Z","document":{"title":"Data Science from Scratch","link":[{"href":"urn:x-pdf:075b70806d7268e551e501c8259b56a7"},{"href":"vault:/Books/Data Science from Scratch.pdf"}],"documentFingerprint":"075b70806d7268e551e501c8259b56a7"},"uri":"vault:/Books/Data Science from Scratch.pdf","target":[{"source":"vault:/Books/Data Science from Scratch.pdf","selector":[{"type":"TextPositionSelector","start":133129,"end":133341},{"type":"TextQuoteSelector","exact":"A  generalization  of  the  median  is  the  quantile,  which  represents  the  value  less  thanwhich a certain percentile of the data lies. (The median represents the value less thanwhich 50% of the data lies.)","prefix":"  (and  outlier)  MichaelJordan.","suffix":"def quantile(x, p):    \"\"\"return"}]}]}
>```
>%%
>*%%PREFIX%%(and  outlier)  MichaelJordan.%%HIGHLIGHT%% ==A  generalization  of  the  median  is  the  quantile,  which  represents  the  value  less  thanwhich a certain percentile of the data lies. (The median represents the value less thanwhich 50% of the data lies.)== %%POSTFIX%%def quantile(x, p):    """return*
>%%LINK%%[[#^a0ndji6soe|show annotation]]
>%%COMMENT%%
>Quantile to filter data based on value range.
>%%TAGS%%
>
^a0ndji6soe
