---
title: Tipo de recurso directoryObjectPartnerReference
description: Representa uma referência a um objeto de diretório em um locatário parceiro. Herda de directoryObject.
author: keylimesoda
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 35cc8be163a9bbbbcdf9330d6b6cf861673e7edf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123786"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>Tipo de recurso directoryObjectPartnerReference

Namespace: microsoft.graph

Representa uma referência a um objeto de diretório em uma organização parceira. Herda de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|description|String| Descrição do objeto retornado. Somente leitura. |
|displayName|Cadeia de caracteres| Nome do objeto de diretório sendo retornado, como grupo ou aplicativo. Somente leitura. |
|externalPartnerTenantId|Guid| O identificador de locatário do locatário parceiro. Somente leitura. |
|id|String| O identificador exclusivo do recurso. Herdado de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0). Somente leitura. |
|objectType|String| O tipo do objeto referenciado no locatário do parceiro. Somente leitura. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObjectPartnerReference"
}-->

```json
{
  "description": "string ",
  "displayName": "string",
  "externalPartnerTenantId": "string (identifier)",
  "id": "string (identifier)",
  "objectType": "string"
}
```

## <a name="see-also"></a>Confira também

- [Obter objetos directory a partir de uma lista de ids](../api/directoryobject-getbyids.md)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
