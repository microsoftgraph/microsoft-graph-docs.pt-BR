---
title: Tipo de recurso accessPackageLocalizedText
description: Um tipo complexo usado para representar uma cadeia de caracteres em um idioma específico.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8d493f0909617dcda26546ccc262d7591c6b9309
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137344"
---
# <a name="accesspackagelocalizedtext-resource-type"></a>Tipo de recurso accessPackageLocalizedText

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo complexo usado para representar uma cadeia de caracteres em um idioma específico.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|languageCode|String|O código ISO para o idioma pretendido. Obrigatório. |
|texto|String|O texto no idioma específico. Obrigatório. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageLocalizedText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageLocalizedText",
  "text": "String",
  "languageCode": "String"
}
```
