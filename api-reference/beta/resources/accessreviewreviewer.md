---
title: Tipo de recurso accessReviewReviewer
description: Representa um revistor que foi contatado para uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f5fbeda2ca839fe07009a46ab2bccd1deb502f17
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259192"
---
# <a name="accessreviewreviewer-resource-type"></a>Tipo de recurso accessReviewReviewer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Objeto que representa as identidades dos revisadores que foram contatados para concluir uma revisão.

Herda da [entidade](entity.md).

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :-------------------------| :---------- | :---------- |
| createdDateTime | DateTimeOffset | A data em que o revistor foi adicionado para a revisão de acesso. |
| displayName | Cadeia de caracteres | Nome do revistor. |
| id | Cadeia de caracteres | Identificador do revistor. Herdado da [entidade](entity.md). |
| userPrincipalName | Cadeia de caracteres | Nome principal do usuário. |


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewReviewer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewer",
  "id": "String",
  "displayName": "String",
  "userPrincipalName": "String",
  "createdDateTime": "String (timestamp)",
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewReviewer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
