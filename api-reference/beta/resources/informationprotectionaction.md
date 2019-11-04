---
title: tipo de recurso informationProtectionAction
description: Descreve a entidade abtract informationProtectionAction.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c0d3bb7ed9464bf4b41d8bd03f6c1835bdce468e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938832"
---
# <a name="informationprotectionaction-resource-type"></a>tipo de recurso informationProtectionAction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **informationProtectionAction** é uma entidade abstrata que é retornada como resultado de qualquer uma das APIs de avaliação de proteção de informações. O objeto contém uma ou mais das ações a seguir que orientam o aplicativo sobre como aplicar, atualizar ou remover o rótulo de proteção de informações. 

* [addContentFooterAction](../resources/addcontentfooteraction.md)
* [addContentHeaderAction](../resources/addcontentheaderaction.md)
* [addwatermarkaction](../resources/addwatermarkaction.md)
* [applyLabelAction](../resources/applylabelaction.md)
* [Personalizada](../resources/customaction.md)
* [justifyaction](../resources/justifyaction.md)
* [metadataaction](../resources/metadataaction.md)
* [protectAdhocAction](../resources/protectadhocaction.md)
* [protectByTemplateAction](../resources/protectbytemplateaction.md)
* [protectionDoNotForwardAction](../resources/protectdonotforwardaction.md)
* [recommendLabelAction](../resources/recommendlabelaction.md)
* [removeContentFooterAction](../resources/removecontentfooteraction.md)
* [removeContentHeaderAction](../resources/removecontentheaderaction.md)
* [removeProtectionAction](../resources/removeprotectionaction.md)
* [removeWatermarkAction](../resources/removewatermarkaction.md)

## <a name="properties"></a>Propriedades

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationProtectionAction",
  "baseType": null
}-->

```json
{

}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->