#
# Docker Container for
# IPython Notebook Server
#
# Dr. Yves J. Hilpisch
# The Python Quants GmbH
#

FROM pythoncontainer

MAINTAINER yves

VOLUME /notebooks
WORKDIR /notebooks

ENV PORT 8888

ADD notebook.sh /
RUN chmod u+x /notebook.sh

ADD Interactive_Widgets.ipynb /notebooks/

CMD /notebook.sh PORT
