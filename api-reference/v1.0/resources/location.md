---
title: Tipo de recurso Location
description: Representa informações de localização para um evento.
localization_priority: Normal
ms.openlocfilehash: 553634aec386798ac17e00b83883c54a99c0f9ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879797"
---
# <a name="location-resource-type"></a>Tipo de recurso Location

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
| locationEmailAddress | Cadeia de caracteres | O endereço de email opcional do local.              |
| locationUri | Cadeia de caracteres | URI opcional que representa o local. |
| locationType | locationType | O tipo de local. Os valores possíveis são: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`. Somente leitura.|
| uniqueId | Cadeia de caracteres | Apenas para uso interno.|
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
