---
title: Tipo de recurso accessReviewReviewer
description: Representa um revistor que foi contatado para uma revisão de acesso.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3a2a51908f73278e592ec02852c96f75570b7646
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162105"
---
# <a name="accessreviewreviewer-resource-type"></a>Tipo de recurso accessReviewReviewer

Namespace: microsoft.graph

Representa as identidades dos revisadores que foram contatados para concluir uma revisão.

Herda da [entidade](entity.md).

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :-------------------------| :---------- | :---------- |
| createdDateTime | DateTimeOffset | A data em que o revistor foi adicionado para a revisão de acesso. |
| displayName | Cadeia de caracteres | Nome do revistor. |
| id | Cadeia de caracteres | Identificador do revistor. Herdado da [entidade](entity.md). |
| userPrincipalName | Cadeia de caracteres | Nome principal do usuário do revistor. |


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
