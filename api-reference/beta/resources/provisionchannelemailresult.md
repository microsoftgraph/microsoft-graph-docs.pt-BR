---
title: Tipo de recurso provisionChannelEmailResult
description: Representa o resultado de uma operação de provisionamento de email de canal.
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ac32dd0db4877dc01a13536689d414b0dcc1175f
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813221"
---
# <a name="provisionchannelemailresult-resource-type"></a>Tipo de recurso provisionChannelEmailResult

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o endereço de email [provisionado](..\api\channel-provisionemail.md) para um [canal](channel.md).

## <a name="properties"></a>Propriedades
| Propriedade | Tipo   | Descrição                               |
| :------- | :----- | :---------------------------------------- |
| email    | Cadeia de caracteres | Representa o endereço de email provisionado. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.provisionChannelEmailResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.provisionChannelEmailResult",
  "email": "String"
}
```
