---
title: Tipo de recurso Location
description: Representa informações de localização para um evento.
ms.localizationpriority: medium
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 678550a8683bf965dbc231055b60bd8a5b95c3df
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134714"
---
# <a name="location-resource-type"></a>Tipo de recurso Location

Namespace: microsoft.graph

Representa informações de localização para um [evento](event.md).

Existem várias maneiras de criar eventos em um calendário, por exemplo, por meio de um aplicativo, usando a API REST [criar evento](../api/user-post-events.md), ou manualmente, usando a interface do usuário do Outlook. Quando você cria um evento usando a interface do usuário, é possível especificar o local como texto sem formatação (por exemplo, "Bar de Harry"), ou na lista de salas fornecida pelo Outlook, pela [Sugestão Automática do Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) ou pela [pesquisa local do Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/). 

Dependendo de como um evento é criado, o Outlook pode definir a propriedade **locationType** somente leitura de maneiras diferentes. 

| Como o evento foi criado  | Propriedade   | Valor esperado |
|:----------|:-------|:--------------------------------|
| API REST [criar evento](../api/user-post-events.md) | **locationType** | `default` |
| Interface do usuário no Outlook | **locationType** | Uma das seguintes opções: <ul><li>`default` para um local inserido como texto sem formatação.</li><li>`conferenceRoom` para uma sala fornecida pela lista de salas do Outlook.</li><li>Ou qualquer uma desta lista (`homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`) para um local da Sugestão Automática do Bing ou da pesquisa local do Bing.</li></ul> |

## <a name="properties"></a>Propriedades
| Propriedade  | Tipo   | Descrição                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| address | [physicalAddress](physicaladdress.md) |O endereço físico do local. |
| coordenadas | [outlookGeoCoordinates](outlookgeocoordinates.md) | As coordenadas geográficas e a elevação do local. |
| displayName  | Cadeia de caracteres | O nome associado ao local.                       |
| locationEmailAddress | String | O endereço de email opcional do local.              |
| locationUri | String | URI opcional que representa o local. |
| locationType | locationType | O tipo de local. Os valores possíveis são: `default` , , , , , , , , , `conferenceRoom` , `homeAddress` `businessAddress` `geoCoordinates` `streetAddress` `hotel` `restaurant` `localBusiness` `postalAddress` . Somente leitura.|
| uniqueId | String | Apenas para uso interno.|
| uniqueIdType | locationUniqueIdType | Apenas para uso interno. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string",
  "locationType": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

