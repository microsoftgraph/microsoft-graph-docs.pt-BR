---
title: Tipo de recurso meetingRegistrationBase
description: Contém informações sobre o registro de reunião base.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 01bdfeaa222464c7e7b44bf5f92482b2b1c3d4e0
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565138"
---
# <a name="meetingregistrationbase-resource-type"></a>Tipo de recurso meetingRegistrationBase

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de registro base de uma reunião online.

Tipo base [de meetingRegistration](meetingregistration.md) [e externalMeetingRegistration](externalmeetingregistration.md).

> [!TIP]
> Esse é um tipo abstrato e não pode ser usado diretamente. Use o tipo derivado [meetingRegistration](meetingregistration.md) [ou externalMeetingRegistration.](externalmeetingregistration.md)

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo                                       | Descrição                                 |
|:------------------|:-------------------------------------------|:--------------------------------------------|
| allowedRegistrant | [meetingAudience](#meetingaudience-values) | Especifica quem pode se registrar na reunião. |

### <a name="meetingaudience-values"></a>valores meetingAudience

| Valor              | Descrição                                                            |
|--------------------|------------------------------------------------------------------------|
| everyone           | Todos podem se registrar na reunião.                                 |
| organização       | Todos na organização do organizador podem se registrar na reunião. |
| unknownFutureValue | Valor de sentinela de enumeração evolvável. Não usar.                      |

## <a name="relationships"></a>Relações

| Relação | Tipo                                                         | Descrição                        |
|:-------------|:-------------------------------------------------------------|:-----------------------------------|
| registrants  | [coleção meetingRegistrantBase](meetingregistrantbase.md) | Registrantes da reunião online. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.meetingRegistrationBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.meetingRegistrationBase",
  "allowedRegistrant": "String",

  "registrants": [{ "@odata.type": "microsoft.graph.meetingRegistrantBase" }]
}
```
