============================================================
 NETWORK DEFENSE PLAN
============================================================

Prepared by:    Phylis
Date:           September 6, 2026
Client:         Maya's Clothing Shop (small retail business)
Engagement:     Network Security Assessment and Remediation Plan


------------------------------------------------------------
 1. ASSESSMENT SUMMARY
------------------------------------------------------------

Maya's Clothing Shop operates a flat network with no
segmentation between payment systems, customer Wi-Fi,
staff devices, and IoT security cameras. Major risks include
weak and publicly exposed Wi-Fi credentials, default router
administrator credentials, outdated IoT devices, and a lack
of monitoring and logging. The most urgent priority is to
separate payment systems from customer and other untrusted
devices while securing the router administration account.


------------------------------------------------------------
 2. NETWORK INVENTORY
------------------------------------------------------------

Device / system          Category          Holds / does

Payment tills x2         Payment           Process customer
                                           transactions

Security cameras x4      IoT               Monitor the shop;
                                           devices are not
                                           regularly updated

Back-office laptop       Data              Stores and accesses
                                           customer/business
                                           information

Maya's laptop            Personal/Business Used for business
                                           activities and
                                           potentially home use

Staff phones x2          Staff             Connect to the
                                           shop Wi-Fi

Smart speaker            IoT               Connected smart
                                           device on the network

Network printer           Infrastructure    Shared business
                                           printing

Customer Wi-Fi            Guest             Provides internet
                                           access to customers
                                           but currently shares
                                           the main network

ISP router                Infrastructure    Provides network
                                           connectivity and
                                           administration


------------------------------------------------------------
 3. PRIORITISED RISKS
------------------------------------------------------------

CRITICAL

  [✓] Flat network: payment tills, customer devices, staff
      devices and IoT devices share the same network. A
      compromised device could potentially provide a path
      toward more sensitive systems.

  [✓] Customer Wi-Fi shares the network with business and
      payment systems, allowing untrusted devices to exist
      on the same network as critical systems.

  [✓] Default router administrator credentials are still
      being used, creating a serious risk of unauthorized
      router configuration.


HIGH

  [✓] Weak shared Wi-Fi password has remained unchanged for
      a long period and is publicly exposed on a chalkboard.
      Unauthorized people can obtain network access.

  [✓] No effective monitoring or logging is in place. A
      security incident could therefore go unnoticed and
      provide little evidence for investigation.


MEDIUM

  [✓] Four security cameras have not been regularly updated.
      Unpatched IoT devices may contain exploitable
      vulnerabilities.

  [✓] The back-office laptop contains business/customer
      information and requires stronger access control and
      least-privilege practices.


LOW

  [✓] The smart speaker is an additional IoT device that is
      not essential to the core payment operation and should
      be isolated from sensitive systems.


------------------------------------------------------------
 4. RECOMMENDED FIXES
------------------------------------------------------------

  - SEGMENT the network into separate logical networks for:
      (a) payment systems,
      (b) customer/guest Wi-Fi,
      (c) IoT/security cameras, and
      (d) staff and office devices.

  - Change the router administrator password from the
    manufacturer's default to a strong, unique password.

  - Update the router firmware and enable automatic updates
    where supported.

  - Configure Wi-Fi using WPA3 where supported, or WPA2 as
    the minimum acceptable option, with a long and unique
    password.

  - Remove the Wi-Fi password from public display and provide
    customers with access through an isolated guest network.

  - Keep payment systems isolated from customer and IoT
    networks and restrict unnecessary communication between
    network segments.

  - Update the security cameras and other IoT devices
    regularly. Replace devices that no longer receive
    security updates.

  - Enable available router/network logging and establish a
    basic process for reviewing important security events.

  - Apply least privilege to the back-office laptop and limit
    access to customer/business information to people who
    actually require it.

  - Review the smart speaker and place it on the IoT network
    rather than allowing it to communicate with sensitive
    business systems.


------------------------------------------------------------
 5. PHASED ACTION PLAN
------------------------------------------------------------

DO FIRST (critical, highest leverage):

  [✓] Change the default router administrator credentials.

  [✓] Separate customer Wi-Fi from payment systems.

  [✓] Create a dedicated network/segment for payment
      devices where the equipment supports it.


THIS WEEK:

  [✓] Replace the publicly displayed Wi-Fi password with a
      strong unique password.

  [✓] Enable WPA3 if supported, or WPA2 with strong
      authentication.

  [✓] Move security cameras and other IoT devices onto a
      separate IoT network.

  [✓] Update router and camera firmware.


THIS MONTH:

  [✓] Enable and review network/router logging.

  [✓] Establish basic monitoring for unusual network activity.

  [✓] Review access permissions on the back-office laptop.

  [✓] Review all connected devices and remove unnecessary
      or unknown devices.

  [✓] Review the smart speaker and other non-essential IoT
      devices.


------------------------------------------------------------
 6. HOW MAYA WILL KNOW IT WORKED
------------------------------------------------------------

Maya can verify that the remediation was successful by
confirming that customer devices can no longer communicate
directly with payment tills or other sensitive business
systems. The router administrator account should use a new
unique password, Wi-Fi should use WPA3 or WPA2 with strong
credentials, and security cameras should be isolated from
payment devices. Network logging should also be active and
reviewed regularly so that suspicious activity can be
detected and investigated.


============================================================
 END OF PLAN
============================================================
