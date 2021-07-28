---
title: Tipo de recurso accessReviewError
description: Representa um erro que ocorreu dentro de um ciclo de vida da instância de revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: dc0fe94daaba28bf92b20cb986760b0d3eb0901b
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534221"
---
# <a name="accessreviewerror-resource-type"></a>Tipo de recurso accessReviewError

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa um erro que ocorreu em um ciclo de vida da instância de revisão de acesso. Esse recurso é somente leitura.

Herda de [genericError](../resources/genericerror.md).

## <a name="properties"></a>Propriedades
| Propriedade                     | Tipo     | Descrição                          |
| :--------------------------- | :------  | :----------                          |
| código  |Cadeia de Caracteres  | Representa o tipo de erro. Herdado de genericError. Somente leitura. |
| mensagem |String | Representa os detalhes do erro. Herdado de genericError. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewError"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
