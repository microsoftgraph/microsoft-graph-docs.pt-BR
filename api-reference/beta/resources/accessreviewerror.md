---
title: Tipo de recurso accessReviewError
description: Representa um erro que ocorreu dentro de um ciclo de vida da instância de revisão de acesso.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7e0b773bd8b1393b160cb666db4d5f19d9501a54
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697922"
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
| código  |Cadeia de caracteres  | Representa o tipo de erro. Herdado de genericError. Somente leitura. |
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
