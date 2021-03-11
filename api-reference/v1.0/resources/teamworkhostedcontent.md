---
title: Tipo de recurso teamworkHostedContent
description: Representa conteúdo rich hospedado pelo Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0a4a4d0a553f77766dd4ddb1f68e27b440fdbf2f
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50634288"
---
# <a name="teamworkhostedcontent-resource-type"></a>Tipo de recurso teamworkHostedContent

Namespace: microsoft.graph

Representa conteúdo rico como imagens e trechos de código no Microsoft Teams. Para conteúdo rico em [mensagens de canal e chat,](chatMessage.md)consulte [chatMessageHostedContent](chatMessageHostedContent.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentBytes|Binária|Somente gravação. Bytes para o conteúdo hospedado (como imagens).|
|contentType|String|Somente gravação. Tipo de conteúdo. sicj como image/png, image/jpg.|
|id|Cadeia de caracteres|ID do conteúdo hospedado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkHostedContent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHostedContent",
  "id": "String (identifier)",
  "contentBytes": "Binary",
  "contentType": "String"
}
```
