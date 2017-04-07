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

Ao criar uma propriedade estendida de valor único ou de vários valores, você pode especificar a **id** em um de dois formatos, com base em um nome de cadeia de caracteres ou em um identificador numérico e como base no tipo real dos valores da propriedade. Como propriedades estendidas interoperam na maioria dos casos com propriedades MAPI definidas não expostas nos metadados da API do Microsoft Graph, para manter a simplicidade, o formato escolhido deve refletir se a propriedade MAPI correspondente usa um valor numérico ou uma cadeia de caracteres em seu [identificador de propriedade MAPI](https://msdn.microsoft.com/en-us/library/office/cc815528.aspx). Você pode encontrar informações sobre o mapeamento de uma propriedade estendida para uma propriedade MAPI existente, como o identificador de propriedade e o GUID, na publicação da Microsoft Corporation \[MS OXPROPS\], ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx).

**Observação** Depois de escolher um formato para a **id**, você deve acessar essa propriedade estendida apenas com esse formato.


**Formatos de id válidos para propriedades estendidas de valor único**

|**Formato**|**Exemplo**|**Descrição**|
|:---------|:----------|:--------------|
| "*{type} {guid} **Nome** {name}*" | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Identifica uma propriedade pelo namespace (o GUID) ao qual ela pertence e por um nome.         |
| "*{type} {guid} **Id** {id}*"     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | Identifica uma propriedade pelo namespace (o GUID) ao qual ela pertence e por um identificador.  |


**Formatos de id válidos para propriedades estendidas de vários valores**

|**Formato**|**Exemplo**|**Descrição**|
|:---------|:----------|:--------------|
| "*{type} {guid} **Nome** {name}*" | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Identifica uma propriedade pelo namespace (o GUID) e por um nome.         |
| "*{type} {guid} **Id** {id}*"     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | Identifica uma propriedade pelo namespace (o GUID) e por um identificador.   |


### <a name="rest-api-operations"></a>Operações da API REST
 
Operações de propriedades estendidas de valor único:

- [Criar uma propriedade estendida em uma instância de recurso nova ou existente](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md)
- [Obter uma instância de recurso, ou uma coleção delas, com uma propriedade estendida usando `$expand` ou `$filter`](../api/singlevaluelegacyextendedproperty_get.md)

Operações de propriedades estendidas de vários valores:

- [Criar uma propriedade estendida em uma instância de recurso nova ou existente](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md)
- [Obter uma instância de recurso com uma propriedade estendida usando `$expand`](../api/multivaluelegacyextendedproperty_get.md).

