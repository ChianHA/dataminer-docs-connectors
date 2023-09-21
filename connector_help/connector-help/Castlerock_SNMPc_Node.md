---
uid: Connector_help_Castlerock_SNMPc_Node
---

# Castlerock SNMPc Node

This connector displays the details of a device connected to the Castlerock SNMPc.

## About

### Version Info

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Range</strong></td>
<td><strong>Key Features</strong></td>
<td><strong>Based on</strong></td>
<td><strong>System Impact</strong></td>
</tr>
<tr class="even">
<td>1.0.0.x</td>
<td><p>This connector is used for <strong>the created DVEs</strong> of one specific node found in the <strong>Node Table</strong> on the <strong>Device page</strong> of the parent connector <strong>Castlerock SNMPc</strong>. Note that the DVE is only created if the specific cell is toggled (see parent connector help page) and this creation can be undone.</p>
<p>This connector is automatically generated by the connector Castlerock SNMPc range 1.0.0.x.</p></td>
<td>-</td>
<td>-</td>
</tr>
<tr class="odd">
<td>2.0.0.x [SLC Main]</td>
<td><p>This connector is used for <strong>the created DVEs</strong> of one specific device found in the <strong>Devices Table</strong> on the <strong>Known IP Addresses page</strong> of the parent connector <strong>Castlerock SNMPc</strong>. Note that the DVE is only created if the specific cell is toggled (see parent connector help page) and there is a view with the same name as the Site Name of the device. This creation can be undone.</p>
<p>This connector is automatically generated by connector Castlerock SNMPc range 2.0.0.x.</p></td>
<td>-</td>
<td>-</td>
</tr>
</tbody>
</table>

### Product Info

| Range     | Supported Firmware     |
|-----------|------------------------|
| 1.0.0.x   | N/A                    |
| 2.0.0.x   | N/A                    |

## Configuration

DVEs running this connector can only be created via the parent connector. More details on how to set up a connection with the device can be found on the connector help page of the parent connector.

## How to use

### Range 1.0.0.x

The **General** page of the connector contains all the raw data that is stored for the node (corresponding to a specific entry in the SNMPc Node Table). The information is updated once every hour.

The **Traps** page is synchronized with the Traps table in the parent connector. However, this page shows only the traps for this specific node. The Map ID is the foreign key used to filter out his data.

This **Info Events** page is synchronized with the Info Events table in the parent connector. However, this page only shows the info events for this specific node. The Map ID is the foreign key used to filter out his data.

### Range 2.0.0.x

This **General** page contains a summary consisting of the IP Address, Device Name, and Site Name of the DVE. Next to this summary, you can find the Traps Table, which is fully synchronized with the Traps Table in the parent connector. However, this table only shows the traps for this specific device. The IP Address is the foreign key used to filter out his data.