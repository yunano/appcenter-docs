.. Copyright (c) 2007-2016 UShareSoft, All rights reserved

.. _appliance-create:

Creating an Appliance Template
------------------------------

You can create either Linux-based or Windows-based appliance templates. The steps differ slightly. Please refer to the appropriate section below.

Creating a Linux-based Appliance
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

To create a new appliance in your private workspace: 

	1. Select the ``VM Builder`` tab and click on ``Create`` in the top right. 
	2. Enter the ``Name`` and ``Version`` of the appliance.  

	.. image:: /images/create-appliance-centos.jpg

	3. From the drop-down menus, select the operating system (distribution, release and architecture).
	4. Click the ``Create`` button. This creates a skeleton of an appliance template in the platform which you can now customize with operating system packages, middleware and application software.
	5. You should now see the appliance overview page. You can add a description to your appliance (optional) and a logo (optional). The logo format must be .jpg, .jpeg or .png.
	6. An OS profile is mandatory. See :ref:`appliance-os-profile-new`. However, you can leave the appliance at this point and edit it later.
	7. If you have made any modifications, click ``save``.

.. note:: When you create an appliance, the packages are stored locally in the UForge cache repository. This ensures that the packages will always be available.

Creating a Windows-based Appliance
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

To create a Windows Appliance:

	1. From the VM Builder tab, select ``Create``.
	2. Enter the appliance name.
	3. Choose ``Windows`` from the OS Distribution drop down menu.
	4. Click ``Create``.
	5. From the ``Stack`` page, select the OS Profile. Each version has a Core or Full release. Click ``Save``.

		.. note:: Once you have chosen the OS Profile, you cannot add any packages or run updates. The OS Profile is static. Once created, if you select OS Profile, you will only be able to view the details of the profile you selected.  

	6. Set the Install profile and click Save.

		.. note:: Unlike Linux, the following cannot be set for Windows appliances: Keyboard, Root user, User & Groups, Kernel Parameters and Firewall.  

	.. image :: /images/windows-install.jpg

	7. Optionally, you can set the Activation Key as part of the Install Profile. If it is not entered in the Install Profile, the default key will be used for a 30-day trial period once the appliance is booted.
	8. Optionally you can add partitions.
		a. Click on Partitioning and select Advanced Partitioning
		b. Click on the green + sign at the top.
		c. You can modify the name and partitions type
		d. Select the filesystem to ntfs and mount point to D: (or such).
		e. Enter the size. The install disk  should be 12 Gb for core versions and not less than 32Gb for the full version
		f. Check the box in the Grow column if you want the partition to be growable.
		g. Click save.

	.. image :: /images/windows-adv-partitions.jpg

	9. Add software bundles from the Project or MySoftware pages.

	Software bundles included in MySoftware and Project will be put on the image disk but the UShareSoft generation tool WILL NOT install them even if these are executable/installers files (.exe, .msi, etc.). It is up to the end user to manually complete the installation of the software bundles.

	For Windows, .exe or .msi files can be given extra parameters. The parameters depend on the .exe or .msi file, and can be used for example for silent installation, providing extra configuration values, etc.

.. note:: A binary called UShareInstallConfig is embedded at generation time, which helps the final user of the Appliance do the last-mile configuration.