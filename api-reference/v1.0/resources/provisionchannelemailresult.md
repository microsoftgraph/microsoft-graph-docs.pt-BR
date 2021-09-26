---
title: Tipo de recurso provisionChannelEmailResult
description: Representa o resultado de uma operação de provisionamento de email de canal.
author: anandab-msft
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d33ebbc5e5584a8969eed6f97bf7f26042e92478
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763692"
---
# <a name="provisionchannelemailresult-resource-type"></a>Tipo de recurso provisionChannelEmailResult

Namespace: microsoft.graph

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
