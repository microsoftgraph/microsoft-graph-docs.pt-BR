---
title: Tipo de recurso directoryObjectPartnerReference
description: Representa uma referência a um objeto de diretório em um locatário parceiro. Herda de directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: dbf1746184c75c9a8ed748b293383679102dbb08664b3cc5f9c90d11c02c6237
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54150000"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>Tipo de recurso directoryObjectPartnerReference

Namespace: microsoft.graph

Representa uma referência a um objeto de diretório em uma organização parceira. Herda de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|description|Cadeia de caracteres| Descrição do objeto retornado. Somente leitura. |
|displayName|String| Nome do objeto de diretório sendo retornado, como grupo ou aplicativo. Somente leitura. |
|externalPartnerTenantId|Guid| O identificador de locatário do locatário parceiro. Somente leitura. |
|id|Cadeia de caracteres| O identificador exclusivo do recurso. Herdado de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0). Apenas leitura. |
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
