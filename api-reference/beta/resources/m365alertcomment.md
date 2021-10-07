---
title: Tipo de recurso m365AlertComment
description: Um comentário gerado por analista associado a um alerta ou incidente.
ms.date: 09/09/2021
author: BenAlfasi
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: c3c59422a8e379bbe7ecf43890774a9474d51b26
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220823"
---
# <a name="m365alertcomment-resource-type"></a>Tipo de recurso m365AlertComment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um comentário gerado por analista associado a um alerta ou incidente. 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|comment|String|O texto do comentário.|
|createdByDisplayName|Cadeia de caracteres|A pessoa ou o nome do aplicativo que enviou o comentário.|
|createdDateTime|DateTimeOffset|A hora em que o comentário foi enviado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.m365AlertComment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.m365AlertComment",
  "comment": "String",
  "createdByDisplayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

