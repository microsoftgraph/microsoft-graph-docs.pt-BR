# <a name="outlook-extended-properties-overview"></a>Visão geral das propriedades estendidas do Outlook

Propriedades estendidas permitem armazenar dados personalizados e servem especificamente como um mecanismo de fallback para os aplicativos acessarem dados personalizados de propriedades MAPI do Outlook quando essas propriedades _ainda não estão expostas nos metadados da API do Microsoft Graph_. Você pode usar a API REST de propriedades estendidas para armazenar ou obter esses dados personalizados nos seguintes recursos de usuário:

- [message](../resources/message.md)
- [mailFolder](../resources/mailfolder.md)
- [event](../resources/event.md)
- [calendar](../resources/calendar.md)
- [contact](../resources/contact.md)
- [contactFolder](../resources/contactfolder.md) 

Ou, nos seguintes recursos de grupo do Office 365:

- grupo [event](../resources/event.md)
- grupo [calendar](../resources/calendar.md)
- grupo [post](../resources/post.md) 

## <a name="use-extended-properties-or-open-extensions"></a>Usar propriedades estendidas ou extensões abertas?

Nos cenários mais comuns, você deve ser capaz de usar extensões abertas (representadas por [openTypeExtension](../resources/opentypeextension.md), anteriormente conhecidas como extensões de dados do Office 365) para armazenar e acessar dados personalizados de instâncias de recursos na caixa de correio do usuário. Use propriedades estendidas somente se você precisar acessar dados personalizados para as propriedades MAPI do Outlook que ainda não estão expostas nos [metadados da API do Microsoft Graph](http://developer.microsoft.com/en-us/graph/docs/overview/call_api). 

## <a name="types-of-extended-properties"></a>Tipos de propriedades estendidas

Dependendo se você pretende armazenar um único valor ou vários valores (do mesmo tipo) em uma propriedade estendida, pode criar uma propriedade estendida como uma [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) ou uma [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md).

Cada um desses tipos identifica a propriedade por sua **id** e armazena dados em **value**. 

Você pode usar **id** para obter uma instância de recurso específica em conjunto com essa propriedade estendida ou para filtrar em uma propriedade estendida de valor único para obter todas as instâncias que possuem essa propriedade. 

**Observação** Não é possível usar a API REST para obter todas as propriedades estendidas de uma instância específica em uma única chamada.
  

### <a name="id-formats"></a>Formatos de id

Você pode especificar o **id** de uma propriedade estendida em um dos três formatos:

- Como uma propriedade nomeada, identificada por um tipo de propriedade estendida, um namespace e um nome em uma sequência de caracteres.
- Como uma propriedade nomeada, identificada por um tipo de propriedade estendida, um namespace e um identificador numérico.
- Em um formato proptag, identificado pelo tipo de propriedade estendida e uma [marca de propriedade MAPI](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).

As próximas 2 tabelas descrevem esses formatos como se aplicam a propriedades estendidas de valor único e múltiplo. {_type_} representa o tipo de valor ou valores da propriedade estendida. Os exemplos mostram tipos de sequência de caracteres, números inteiros e matrizes.

**Formatos de id válidos para propriedades estendidas de valor único**

|**Formato**|**Exemplo**|**Descrição**|
|:---------|:----------|:--------------|
| "{_type_} {_guid_} **Name** {_name_}" | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Identifica uma propriedade pelo namespace (o GUID) ao qual ela pertence e por um nome.         |
| "{_type_} {_guid_} **Id** {_id_}"     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | Identifica uma propriedade pelo namespace (o GUID) ao qual ela pertence e por um identificador numérico.  |
| "{_type_} {_proptag_}"                    | ```"String 0x4001001E"```                                           | Identifica uma propriedade pré-definida pela sua marca de propriedade. |

**Formatos de id válidos para propriedades estendidas de valores múltiplos**

|**Formato**|**Exemplo**|**Descrição**|
|:---------|:----------|:--------------|
| "{_type_} {_guid_} **Name** {_name_}" | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Identifica uma propriedade pelo namespace (o GUID) ao qual ela pertence e por um nome.         |
| "{_type_} {_guid_} **Id** {_id_}"     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | Identifica uma propriedade pelo namespace (o GUID) ao qual ela pertence e por um identificador numérico.   |
| "{_type_} {_proptag_}"                    | ```"StringArray 0x4002101E"```                                           | Identifica uma propriedade pré-definida pela sua marca de propriedade. |


Use um dos formatos de nome da propriedade para definir uma propriedade estendida de valor único ou múltiplo como uma propriedade personalizada. Dentre os dois formatos, o primeiro que recebe um nome em sequência de caracteres (**Name**) é o preferido para facilitar a referência. Propriedades nomeadas têm seus [identificadores de propriedade](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) no intervalo 0x8000-0xfffe.

Use o formato proptag para acessar as propriedades predefinidas por MAPI ou por um cliente ou servidor que ainda não foi exposto no Microsoft Graph. Essas propriedades têm identificadores no intervalo 0x0001-0x7fff. Não tente definir uma propriedade personalizada usando o formato de proptag. 

Você pode encontrar informações sobre o mapeamento de uma propriedade estendida para uma propriedade MAPI existente, como o identificador de propriedade e o GUID, na publicação da Microsoft Corporation \[MS-OXPROPS\], ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx).

**Observação** Depois de escolher um formato para a **id**, você deve acessar essa propriedade estendida apenas com esse formato.

### <a name="rest-api-operations"></a>Operações da API REST
 
Operações de propriedades estendidas de valor único:

- [Criar uma propriedade estendida em uma instância de recurso nova ou existente](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md)
- [Obter uma instância de recurso, ou uma coleção delas, com uma propriedade estendida usando `$expand` ou `$filter`](../api/singlevaluelegacyextendedproperty_get.md)

Operações de propriedades estendidas de vários valores:

- [Criar uma propriedade estendida em uma instância de recurso nova ou existente](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md)
- [[Obter uma instância de recurso com uma propriedade estendida usando `$expand`](../api/multivaluelegacyextendedproperty_get.md). `$expand`](../api/multivaluelegacyextendedproperty_get.md)

