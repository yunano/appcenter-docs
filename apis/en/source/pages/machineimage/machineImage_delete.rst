.. Copyright 2016 FUJITSU LIMITED

.. _machineImage-delete:

machineImage_delete
-------------------

.. function:: DELETE /users/{uid}/appliances/{aid}/images/{itid}

.. sidebar:: Summary

	* Method: ``DELETE``
	* Response Code: ``204 / 200``
	* Response Formats: 
	* Since: ``UForge 1.0``

Deletes a machine image generated from an appliance.

Security Summary
~~~~~~~~~~~~~~~~

* Requires Authentication: ``true``
* Entitlements Required: ``appliance_create``

URI Parameters
~~~~~~~~~~~~~~

* ``uid`` (required): the user name (login name) of the :ref:`user-object`
* ``itid`` (required): the id of the :ref:`image-object`
* ``aid`` (required): the id of the :ref:`appliance-object`

HTTP Request Body Parameters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

None

Example Request
~~~~~~~~~~~~~~~

.. code-block:: bash

	curl "https://uforge.example.com/api/users/{uid}/appliances/{aid}/images/{itid}" -X DELETE \
	-u USER_LOGIN:PASSWORD -H "Accept: application/xml"

.. seealso::

	 * :ref:`appliance-object`
	 * :ref:`image-object`
	 * :ref:`imagepkgs-object`
	 * :ref:`machineImage-deleteAll`
	 * :ref:`machineImage-download`
	 * :ref:`machineImage-downloadFile`
	 * :ref:`machineImage-generate`
	 * :ref:`machineImage-get`
	 * :ref:`machineImage-getAll`
	 * :ref:`machineImage-regenerate`
	 * :ref:`machineImageGeneration-cancel`
	 * :ref:`machineImageStatus-getAll`
	 * :ref:`machineImageStatus-get`
	 * :ref:`machineImagePkg-getAll`
	 * :ref:`machineImage-publish`
	 * :ref:`machineImagePublish-cancel`
	 * :ref:`machineImagePublished-get`
	 * :ref:`machineImagePublished-getAll`
	 * :ref:`machineImagePublished-delete`
	 * :ref:`machineImagePublished-deleteAll`
	 * :ref:`machineImagePublished-download`
	 * :ref:`machineImagePublishedStatus-get`
	 * :ref:`machineImagePublishedStatus-getAll`
	 * :ref:`applianceImage-publish`
