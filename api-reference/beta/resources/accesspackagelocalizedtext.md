---
title: tipo de recurso accessPackageLocalizedText
description: Um tipo complexo usado para representar uma cadeia de caracteres em um idioma específico.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9573ae4118f02abdba5686fd94da96da71d374c2
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720070"
---
# <a name="accesspackagelocalizedtext-resource-type"></a>tipo de recurso accessPackageLocalizedText

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo complexo usado para representar uma cadeia de caracteres em um idioma específico.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Campo|Cadeia de caracteres|O código ISO do idioma desejado. Obrigatório. |
|texto|Cadeia de caracteres|O texto no idioma específico. Obrigatório. |

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
