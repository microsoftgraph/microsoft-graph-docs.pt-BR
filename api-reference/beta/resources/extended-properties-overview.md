---
title: Visão geral das propriedades estendidas do Outlook
description: 'Propriedades estendidas permitem o armazenamento de dados personalizados e especificamente servem como um mecanismo de fallback para os aplicativos acessarem '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: 407f9e9fcc8f2ce46ad714f6ab425345356c57ab
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129482"
---
# <a name="outlook-extended-properties-overview"></a>Visão geral das propriedades estendidas do Outlook

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

Propriedades estendidas permitem armazenar dados personalizados e servem especificamente como um mecanismo de fallback para os aplicativos acessarem dados personalizados de propriedades MAPI do Outlook quando essas propriedades _ainda não estão expostas nos metadados da API do Microsoft Graph_. Você pode usar a API REST de propriedades estendidas para armazenar ou obter esses dados personalizados nos seguintes recursos de usuário:

- [message](../resources/message.md)
- [mailFolder](../resources/mailfolder.md)
- [event](../resources/event.md)
- [calendar](../resources/calendar.md)
- [contact](../resources/contact.md)
- [contactFolder](../resources/contactfolder.md)
- [Tarefa do Outlook](../resources/outlooktask.md)
- [Pasta de tarefas do Outlook](../resources/outlooktaskfolder.md)

Ou, nos seguintes recursos de grupo do Microsoft 365:

- grupo [event](../resources/event.md)
- grupo [calendar](../resources/calendar.md)
- grupo [post](../resources/post.md)

## <a name="use-extended-properties-or-open-extensions"></a>Usar propriedades estendidas ou extensões abertas?

Nos cenários mais comuns, você deve ser capaz de usar extensões abertas (representadas por [openTypeExtension](../resources/opentypeextension.md), anteriormente conhecidas como extensões de dados do Office 365) para armazenar e acessar dados personalizados de instâncias de recursos na caixa de correio do usuário. Use propriedades estendidas somente se você precisar acessar dados personalizados para as propriedades MAPI do Outlook que ainda não estão expostas nos [metadados da API do Microsoft Graph](../index.md).

## <a name="types-of-extended-properties"></a>Tipos de propriedades estendidas

Dependendo se você pretende armazenar um único valor ou vários valores (do mesmo tipo) em uma propriedade estendida, pode criar uma propriedade estendida como uma [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) ou uma [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).

Cada um desses tipos identifica a propriedade por sua **id** e armazena dados em **value**.

Você pode usar **id** para obter uma instância de recurso específica em conjunto com essa propriedade estendida ou para filtrar em uma propriedade estendida de valor único para obter todas as instâncias que possuem essa propriedade.

**Observação** Não é possível usar a API REST para obter todas as propriedades estendidas de uma instância específica em uma única chamada.


### <a name="id-formats"></a>formatos de id

Você pode especificar o **id** de uma propriedade estendida em um dos três formatos:

- Como uma propriedade nomeada, identificada pelo tipo de propriedade estendida, namespace e nome de uma cadeia de caracteres.
- Como uma propriedade nomeada, identificada pelo tipo de propriedade estendida, namespace e um identificador numérico.
- Em um formato de proptag, identificado pelo tipo de propriedade estendida e uma [marca de propriedade MAPI](/office/client-developer/outlook/mapi/mapi-property-tags).

As próximas 2 tabelas descrevem esses formatos aplicados a propriedades estendidas única e com vários valores. {_tipo_} representa o tipo de valor ou valores da propriedade estendida. Os exemplos mostram a cadeia de caracteres, inteiro e matrizes desses tipos.

**Formatos de id válidos para propriedades estendidas de valor único**

|**Formato**|**Exemplo**|**Descrição**|
|:---------|:----------|:--------------|
| "{_type_} {_guid_} **Name** {_name_}" | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Identifica uma propriedade namespace (GUID) à qual ele pertence, e um nome de cadeia de caracteres.         |
| "{_type_} {_guid_} **Id** {_id_}"     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | Identifica uma propriedade namespace (GUID) à qual ele pertence, e um identificador numérico.  |
| "{_type_} {_proptag_}"                    | ```"String 0x4001001E"```                                           | Identifica uma propriedade predefinida por sua marca de propriedade. |

**Formatos de id válidos para propriedades estendidas de vários valores**

|**Formato**|**Exemplo**|**Descrição**|
|:---------|:----------|:--------------|
| "{_type_} {_guid_} **Name** {_name_}" | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Identifica uma propriedade namespace (GUID) e um nome de cadeia de caracteres.         |
| "{_type_} {_guid_} **Id** {_id_}"     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | Identifica uma propriedade namespace (GUID) e um identificador numérico.   |
| "{_type_} {_proptag_}"                    | ```"StringArray 0x4002101E"```                                           | Identifica uma propriedade predefinida por sua marca de propriedade. |


Use qualquer um dos formatos de propriedade nomeada para definir uma propriedade estendida de valor único ou vários valores como uma propriedade personalizada. Entre os dois formatos, o primeiro que leva o nome da cadeia de caracteres (**Nome**) é o formato preferencial para facilitar a referência. Propriedades nomeadas tem seus [identificadores de propriedade](/office/client-developer/outlook/mapi/mapi-property-identifier-overview) no intervalo 0x8000-0xfffe.

Use o formato proptag para acessar propriedades predefinidas por MAPI ou por um cliente ou servidor e que já não tenha sido exibida no Microsoft Graph. Essas propriedades tem identificadores de propriedade no intervalo 0x0001-0x7fff. Não tente definir uma propriedade personalizada usando o formato proptag.

Você pode encontrar informações sobre o mapeamento de uma propriedade estendida para uma propriedade MAPI existente, como o identificador de propriedade e o GUID, na publicação da Microsoft Corporation \[MS-OXPROPS\], ["Exchange Server Protocols Master Property List"](/openspecs/exchange_server_protocols/ms-oxprops/f6ab1613-aefe-447d-a49c-18217230b148).

**Observação** Depois de escolher um formato para a **id**, você deve acessar essa propriedade estendida apenas com esse formato.

## <a name="rest-api-operations"></a>Operações da API REST

Operações de propriedades estendidas de valor único:

- [Criar uma propriedade estendida em uma instância de recurso nova ou existente](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [Obter uma instância de recurso, ou uma coleção delas, com uma propriedade estendida usando `$expand` ou `$filter`](../api/singlevaluelegacyextendedproperty-get.md)

Operações de propriedades estendidas de vários valores:

- [Criar uma propriedade estendida em uma instância de recurso nova ou existente](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [Obter uma instância de recurso com uma propriedade estendida usando `$expand`](../api/multivaluelegacyextendedproperty-get.md).