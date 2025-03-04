# Schema Types

<details>
  <summary><strong>Table of Contents</strong></summary>

  * [Query](#query)
  * [Objects](#objects)
    * [Organization](#organization)
    * [Person](#person)
  * [Scalars](#scalars)
    * [Boolean](#boolean)
    * [ID](#id)
    * [Int](#int)
    * [String](#string)
  * [Unions](#unions)
    * [Party](#party)

</details>

## Query
<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong><a name="party">party</a></strong></td>
<td valign="top"><a href="#party">Party</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#id">ID</a>!</td>
<td></td>
</tr>
</tbody>
</table>

## Objects

### Organization

A group of persons working together for a purpose

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong><a name="id">id</a></strong></td>
<td valign="top"><a href="#id">ID</a>!</td>
<td>

Node ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong><a name="name">name</a></strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Name of the organization

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong><a name="email">email</a></strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Main contact email address

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong><a name="founded">founded</a></strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Date the organization was founded

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong><a name="ceo">ceo</a></strong></td>
<td valign="top"><a href="#person">Person</a></td>
<td>

The CEO

</td>
</tr>
</tbody>
</table>

### Person

A human being

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong><a name="id">id</a></strong></td>
<td valign="top"><a href="#id">ID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong><a name="firstname">firstName</a></strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong><a name="lastname">lastName</a></strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong><a name="email">email</a></strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong><a name="age">age</a></strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong><a name="dob">dob</a></strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

## Scalars

### Boolean

The `Boolean` scalar type represents `true` or `false`.

### ID

The `ID` scalar type represents a unique identifier, often used to refetch an object or as key for a cache. The ID type appears in a JSON response as a String; however, it is not intended to be human-readable. When expected as an input type, any string (such as `"4"`) or integer (such as `4`) input value will be accepted as an ID.

### Int

The `Int` scalar type represents non-fractional signed whole numeric values. Int can represent values between -(2^31) and 2^31 - 1.

### String

The `String` scalar type represents textual data, represented as UTF-8 character sequences. The String type is most often used by GraphQL to represent free-form human-readable text.


## Unions

### Party

Either a person or an organization

<table>
<thead>
<th align="left">Type</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong><a href="#person">Person</a></strong></td>
<td valign="top">A human being</td>
</tr>
<tr>
<td valign="top"><strong><a href="#organization">Organization</a></strong></td>
<td valign="top">A group of persons working together for a purpose</td>
</tr>
</tbody>
</table>
