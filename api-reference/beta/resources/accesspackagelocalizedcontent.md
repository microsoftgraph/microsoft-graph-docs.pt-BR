---
title: Tipo de recurso accessPackageLocalizedContent
description: Um tipo complexo usado para representar texto em localidades diferentes, juntamente com um texto padrão.*
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 155d0ffd8f7f705c79bd753aa26f659968b87829
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137351"
---
# <a name="accesspackagelocalizedcontent-resource-type"></a>Tipo de recurso accessPackageLocalizedContent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo complexo usado para representar um texto em vários formulários localizados. Ele inclui um texto padrão, que é usado em qualquer caso em que a localização solicitada não está disponível.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|defaultText|String|A cadeia de caracteres de fallback, que é usada quando uma localização solicitada não está disponível. Obrigatório. |
|localizedTexts|[Coleção accessPackageLocalizedText](../resources/accesspackagelocalizedtext.md)|Conteúdo representado em um formato para uma localidade específica. |

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
