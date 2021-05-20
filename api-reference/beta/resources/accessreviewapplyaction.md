---
title: Tipo de recurso accessReviewApplyAction
description: Representa a ação a ser tomada em usuários revisados após a conclusão de uma instância de revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c7f1425bb7155762f973f65fd766db8da55b8d77
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579638"
---
# <a name="accessreviewapplyaction-resource-type"></a>Tipo de recurso accessReviewApplyAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa uma classe base para aplicar ações [no accessReviewScheduleSettings](accessreviewschedulesettings.md) de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md). Tipos derivados com suporte:

- [removeAccessApplyAction](removeaccessapplyaction.md) é um tipo derivado de accessReviewApplyAction que indica a remoção do acesso de uma entidade que está sendo revisada após a conclusão da revisão. Esse é o tipo padrão para a propriedade applyActions em accessReviewScheduleSettings e não precisa ser especificado.

- [disableAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) é um tipo derivado de accessReviewApplyAction que indica desabilitar e excluir o usuário que está sendo revisado após a conclusão da revisão. Esse é o tipo não padrão e precisa ser especificado em accessReviewScheduleSettings.

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
