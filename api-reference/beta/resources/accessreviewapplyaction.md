---
title: tipo de recurso accessReviewApplyAction
description: Representa a ação a ser tomada nos usuários revisados após a conclusão de uma instância de revisão do Access.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 33aa0f7a9d7fbfeab9b957f4c94b87d6f6e50d44
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000768"
---
# <a name="accessreviewapplyaction-resource-type"></a>tipo de recurso accessReviewApplyAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma classe base para aplicar ações no [accessReviewScheduleSettings](accessreviewschedulesettings.md) de um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md). Tipos derivados suportados:

- **removeAccessApplyAction** é um tipo derivado de accessReviewApplyAction que indica remover o acesso de uma entidade que está sendo revisada após a conclusão da revisão. Este é o tipo padrão para a propriedade applyActions em accessReviewScheduleSettings e não precisa ser especificado.

- **disableAndDeleteUserApplyAction** é um tipo derivado de accessReviewApplyAction que indica desabilitar e excluir o usuário que está sendo revisado após a conclusão da revisão. Este é o tipo não padrão e precisa ser especificado em accessReviewScheduleSettings.

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
