---
title: Tipo de recurso accessReviewReviewer
description: Representa um revisores que foi contatado para uma revisão de acesso.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 63d07f913641f0eb8c0a6aeec8f153395ea54ca2
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698097"
---
# <a name="accessreviewreviewer-resource-type"></a>Tipo de recurso accessReviewReviewer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Objeto que representa as identidades dos revisores que foram contatados para concluir uma revisão.

Herda de [entidade](entity.md).

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
