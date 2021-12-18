---
title: Tipo de recurso meetingRegistrantBase
description: Representa um registro de reunião base que se registrou em uma reunião online.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c17ccf2cb3b34b9b139726b727cd84148b6bc9a8
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565150"
---
# <a name="meetingregistrantbase-resource-type"></a>Tipo de recurso meetingRegistrantBase

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um registro de reunião base que se registrou em uma reunião online.

Tipo base [de meetingRegistrant](meetingregistrant.md) [e externalMeetingRegistrant](externalmeetingregistrant.md).

> [!TIP]
> Esse é um tipo abstrato e não pode ser usado diretamente. Use o tipo derivado [meetingRegistrant](meetingregistrant.md) [ou externalMeetingRegistrant.](externalmeetingregistrant.md)

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo   | Descrição                                                         |
|:-----------|:-------|:--------------------------------------------------------------------|
| id         | Cadeia de caracteres | O identificador exclusivo do registro. Somente leitura.                 |
| joinWebUrl | Cadeia de caracteres | Uma URL da Web exclusiva para o registro ingressar na reunião. Somente leitura. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.meetingRegistrantBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.meetingRegistrantBase",
  "id": "String (identifier)",
  "joinWebUrl": "String"
}
```
