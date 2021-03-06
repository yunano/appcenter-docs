.. Copyright 2016 FUJITSU LIMITED

.. _appliance-publish-machine-image:

Publishing a Machine Image
--------------------------

In order to publish a machine image to a cloud environment, you must already have credentials to access that environment. 

	1. If not already done, create a new cloud account for the target environment.  For more information, see :ref:`account-cloud-accounts`. 
	2. Go to the appliance and click the ``Machine Images`` page. If you have not generated a machine image, you will need to do so as described in :ref:`appliance-generate-machine-image`.
	3. Click on the arrow to publish your image.

		.. image:: /images/machine-image-publish.png

	4. Following the instructions, choose the cloud account to use and fill in any additional information required.
	5. Click ``publish``.

	.. note:: Publishing an image to Amazon will launch an instance and therefore will be billed to the user account. Azure trial accounts are not supported for publishing images from UForge. Only full Azure accounts can be used. 

	6. The publication will take a few minutes to complete (depending on the size of the image and the network connectivity between UForge and the target cloud environment). The publication progress is shown. At the end of the publication, the machine image has been published by UForge to your target cloud environment. The published image can be found in the target cloud environment.

	.. note:: UForge does not launch instances in the target cloud environment. If you wish to launch an instance from this machine image, you should go to your target cloud environment console for further actions.
