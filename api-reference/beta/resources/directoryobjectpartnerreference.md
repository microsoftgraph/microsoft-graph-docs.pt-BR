---
title: Tipo de recurso directoryObjectPartnerReference
description: Representa uma referência a um objeto de diretório em um locatário parceiro. Herda de directoryObject.
author: keylimesoda
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 0b8825a7bd20e7e76aa3825cf29e8b7246e3ad8a
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62855074"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>Tipo de recurso directoryObjectPartnerReference

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma referência a um objeto de diretório em uma organização parceira. Herda de [directoryObject](directoryobject.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|description|String| Descrição do objeto retornado. Somente leitura. |
|displayName|String| Nome do objeto de diretório sendo retornado, como grupo ou aplicativo. Somente leitura. |
|externalPartnerTenantId|GUID| O identificador de locatário do locatário parceiro. Somente leitura. |
|id|String| O identificador exclusivo do recurso. Herdado de [directoryObject](directoryobject.md). Somente leitura. |
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
