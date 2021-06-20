---
title: Tipo de recurso accessReviewApplyAction
description: Representa a ação a ser tomada em usuários revisados após a conclusão de uma instância de revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4a96ed1009a8af4404c50041258e784d8bd04030
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030971"
---
# <a name="accessreviewapplyaction-resource-type"></a>Tipo de recurso accessReviewApplyAction

Namespace: microsoft.graph

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

