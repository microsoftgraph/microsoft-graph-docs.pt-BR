---
title: tipo de recurso accessPackageLocalizedContent
description: Um tipo complexo usado para representar texto em diferentes locais, juntamente com um texto padrão. *
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 91ef87428b4171317943e9ecf1ec92e959c7a62b
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720052"
---
# <a name="accesspackagelocalizedcontent-resource-type"></a>tipo de recurso accessPackageLocalizedContent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo complexo usado para representar um texto em vários formulários do localalized. Ele inclui um texto padrão, que é usado em qualquer caso em que a localização solicitada não está disponível.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|defaultText|Cadeia de caracteres|A cadeia de caracteres de fallback, que é usada quando uma localização solicitada não está disponível. Obrigatório. |
|localizedTexts|coleção [accessPackageLocalizedText](../resources/accesspackagelocalizedtext.md)|Conteúdo representado em um formato para uma localidade específica. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageLocalizedContent",
  "defaultText": "String",
  "localizedTexts": [
    {
      "@odata.type": "microsoft.graph.accessPackageLocalizedText"
    }
  ]
}
```
