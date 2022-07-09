---
title: Tipo de recurso accessReviewApplyAction
description: Representa a ação a ser tomada em usuários revisados após a conclusão de uma instância de revisão de acesso.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c88cc607cedb23be344ac5bb33573dedaadb1467
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698160"
---
# <a name="accessreviewapplyaction-resource-type"></a>Tipo de recurso accessReviewApplyAction

Namespace: microsoft.graph

Representa uma classe base para aplicar ações [no accessReviewScheduleSettings](accessreviewschedulesettings.md) de um [objeto accessReviewScheduleDefinition](accessreviewscheduledefinition.md) . Há suporte para os seguintes tipos derivados:

- [removeAccessApplyAction](removeaccessapplyaction.md) indica a remoção do acesso de uma entidade que está sendo revisada após a conclusão da revisão. Esse é o tipo padrão para a propriedade applyActions em accessReviewScheduleSettings e não precisa ser especificado.

- [disableAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) indica desabilitar e excluir o usuário que está sendo examinado após a conclusão da revisão. Esse é o tipo não padrão e deve ser especificado explicitamente em accessReviewScheduleSettings.

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

