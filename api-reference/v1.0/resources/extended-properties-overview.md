---
title: Visão geral das propriedades estendidas do Outlook
description: 'Propriedades estendidas permitem armazenar dados personalizados e especificamente servem como um mecanismo de fallback para aplicativos acessar '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 935f97819155318a6bfc7c77d07bf8a308e512e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949567"
---
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

Nos cenários mais comuns, você deve ser capaz de usar extensões abertas (representadas por [openTypeExtension](../resources/opentypeextension.md), anteriormente conhecidas como extensões de dados do Office 365) para armazenar e acessar dados personalizados de instâncias de recursos na caixa de correio do usuário. Use propriedades estendidas somente se você precisar acessar dados personalizados para as propriedades MAPI do Outlook que ainda não estão expostas nos [metadados da API do Microsoft Graph](https://developer.microsoft.com/graph/docs/overview/call_api). 

## <a name="types-of-extended-properties"></a>Tipos de propriedades estendidas

Dependendo se você pretende armazenar um único valor ou vários valores (do mesmo tipo) em uma propriedade estendida, pode criar uma propriedade estendida como uma [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) ou uma [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).

Cada um desses tipos identifica a propriedade por sua **id** e armazena dados em **value**. 

Você pode usar **id** para obter uma instância de recurso específica em conjunto com essa propriedade estendida ou para filtrar em uma propriedade estendida de valor único para obter todas as instâncias que possuem essa propriedade. 

**Observação** Não é possível usar a API REST para obter todas as propriedades estendidas de uma instância específica em uma única chamada.
  

### <a name="id-formats"></a>formatos de ID

Você pode especificar o **id** de uma propriedade estendida em um dos três formatos:

- Como uma propriedade nomeada, identificada por um nome de cadeia de caracteres, namespace e o tipo de propriedade estendida.
- Como uma propriedade nomeada, identificada por um identificador numérico, namespace e o tipo de propriedade estendida.
- Em um formato proptag, identificado pelo tipo de propriedade estendida e uma [marca de propriedade MAPI](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).

As tabelas próximas 2 descrevem esses formatos como propriedades estendidas aplicadas ao único e de valores múltiplos. {_tipo_} representa o tipo do valor ou valores da propriedade estendida. Os exemplos mostram a cadeia de caracteres, inteiro e matrizes desses tipos.

**Formatos de id válidos para propriedades estendidas de valor único**

|**Formato**|**Exemplo**|**Descrição**|
|:---------|:----------|:--------------|
| "{_type_} {_guid_} **Name** {_name_}" | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Identifica uma propriedade namespace (o GUID) qual ele pertence e um nome de cadeia de caracteres.         |
| "{_type_} {_guid_} **Id** {_id_}"     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | Identifica uma propriedade namespace (o GUID) qual ele pertence e um identificador numérico.  |
| "{_tipo_} {_proptag_}"                    | ```"String 0x4001001E"```                                           | Identifica uma propriedade pré-definidos pela marca de sua propriedade. |

**Formatos de id válidos para propriedades estendidas de vários valores**

|**Formato**|**Exemplo**|**Descrição**|
|:---------|:----------|:--------------|
| "{_type_} {_guid_} **Name** {_name_}" | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Identifica uma propriedade por namespace (o GUID) e um nome de cadeia de caracteres.         |
| "{_type_} {_guid_} **Id** {_id_}"     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | Identifica uma propriedade por namespace (o GUID) e um identificador numérico.   |
| "{_tipo_} {_proptag_}"                    | ```"StringArray 0x4002101E"```                                           | Identifica uma propriedade pré-definidos pela marca de sua propriedade. |


Use um dos formatos de nome da propriedade para definir uma propriedade estendida de valor único ou vários valor como uma propriedade personalizada. Entre os dois formatos, o primeiro que necessita de um nome de cadeia de caracteres (**nome**) é o formato preferido para facilitar a referência. Propriedades nomeadas tem seus [identificadores de propriedade](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) em 0x8000-0xfffe o intervalo.

Use o formato de proptag para acessar as propriedades predefinidas por MAPI ou por um cliente ou servidor e que já não foram expostas no Microsoft Graph. Essas propriedades têm identificadores de propriedade no 0x0001-0x7fff intervalo. Não tente definir uma propriedade personalizada usando o formato de proptag. 

Você pode encontrar informações sobre o mapeamento de uma propriedade estendida para uma propriedade MAPI existente, como o identificador de propriedade e o GUID, na publicação da Microsoft Corporation \[MS-OXPROPS\], ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).

**Observação** Depois de escolher um formato para a **id**, você deve acessar essa propriedade estendida apenas com esse formato.

### <a name="rest-api-operations"></a>Operações da API REST
 
Operações de propriedades estendidas de valor único:

- [Criar uma propriedade estendida em uma instância de recurso nova ou existente](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [Obter uma instância de recurso, ou uma coleção delas, com uma propriedade estendida usando `$expand` ou `$filter`](../api/singlevaluelegacyextendedproperty-get.md)

Operações de propriedades estendidas de vários valores:

- [Criar uma propriedade estendida em uma instância de recurso nova ou existente](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [Obter uma instância de recurso com uma propriedade estendida usando `$expand`](../api/multivaluelegacyextendedproperty-get.md).

