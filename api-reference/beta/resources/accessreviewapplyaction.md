---
title: Tipo de recurso accessReviewApplyAction
description: Representa a ação a ser tomada em usuários revisados após a conclusão de uma instância de revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7360c2a3a058eb4f884cb786c05a83efe09a6193
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133536"
---
# <a name="accessreviewapplyaction-resource-type"></a>Tipo de recurso accessReviewApplyAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma classe base para aplicar ações em [accessReviewScheduleSettings](accessreviewschedulesettings.md) de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md). Tipos derivados com suporte:

- **removeAccessApplyAction** é um tipo derivado de accessReviewApplyAction que indica a remoção do acesso de uma entidade que está sendo revisada após a conclusão da revisão. Esse é o tipo padrão para a propriedade applyActions em accessReviewScheduleSettings e não precisa ser especificado.

- **disableAndDeleteUserApplyAction** é um tipo derivado de accessReviewApplyAction que indica desabilitar e excluir o usuário que está sendo revisado após a conclusão da revisão. Esse é o tipo não padrão e precisa ser especificado em accessReviewScheduleSettings.

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewApplyAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewApplyAction"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewApplyAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
