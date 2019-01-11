---
title: tipo de recurso de directoryObjectPartnerReference
description: Representa uma referência a um objeto de diretório em um locatário de parceiro. Herda de directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 46d0f749ac77e7d51e03314e78cfccf494dcc6fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884858"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>tipo de recurso de directoryObjectPartnerReference

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa uma referência a um objeto de diretório em uma organização parceira. Herda de [directoryObject](directoryobject.md?view=graph-rest-beta).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|description|Cadeia de caracteres| Descrição do objeto retornado. Somente leitura. |
|displayName|Cadeia de caracteres| Nome do objeto de diretório retornado, como o grupo ou aplicativo. Somente leitura. |
|externalPartnerTenantId|Guid| O identificador do locatário para o locatário de parceiro. Somente leitura. |
|id|Cadeia de caracteres| O identificador exclusivo para o recurso. Herdado de [directoryObject](directoryobject.md?view=graph-rest-beta). Somente leitura. |
|objectType|String| O tipo do objeto referenciado no locatário parceiro. Somente leitura. |

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

- [Obter objetos directory a partir de uma lista de ids](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
