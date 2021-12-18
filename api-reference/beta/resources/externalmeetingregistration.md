---
title: Tipo de recurso externalMeetingRegistration
description: Contém informações sobre o registro de reunião externa.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: af59114df32f24c36c1cd8d75e344162ac6e0d88
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565151"
---
# <a name="externalmeetingregistration-resource-type"></a>Tipo de recurso externalMeetingRegistration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes do registro externo de uma reunião online.

Herda de [meetingRegistrationBase](meetingregistrationbase.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar externalMeetingRegistration](../api/externalmeetingregistration-post.md)|[externalMeetingRegistration](externalmeetingregistration.md)|Crie um novo [objeto externalMeetingRegistration.](externalmeetingregistration.md)|
|[Obter externalMeetingRegistration](../api/externalmeetingregistration-get.md)|[externalMeetingRegistration](externalmeetingregistration.md)|Leia as propriedades e as relações de um [objeto externalMeetingRegistration.](externalmeetingregistration.md)|
|[Excluir externalMeetingRegistration](../api/externalmeetingregistration-delete.md)|Nenhum|[Exclua um objeto externalMeetingRegistration.](externalmeetingregistration.md)|

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo                                       | Descrição                                 |
|:------------------|:-------------------------------------------|:--------------------------------------------|
| allowedRegistrant | [meetingAudience](#meetingaudience-values) | Especifica quem pode se registrar na reunião. Herdado [de meetingRegistrationBase](meetingregistrationbase.md). |

### <a name="meetingaudience-values"></a>valores meetingAudience

| Valor              | Descrição                                                            |
|--------------------|------------------------------------------------------------------------|
| everyone           | Todos podem se registrar na reunião.                                 |
| organização       | Todos na organização do organizador podem se registrar na reunião. |
| unknownFutureValue | Valor de sentinela de enumeração evolvável. Não usar.                      |

## <a name="relationships"></a>Relações

| Relação | Tipo                                                                 | Descrição                        |
|:-------------|:---------------------------------------------------------------------|:-----------------------------------|
| registrants  | [Coleção externalMeetingRegistrant](externalmeetingregistrant.md) | Registrantes da reunião online. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalMeetingRegistration",
  "baseType": "microsoft.graph.meetingRegistrationBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalMeetingRegistration",
  "allowedRegistrant": "String",

  "registrants": [{ "@odata.type": "microsoft.graph.externalMeetingRegistrant" }]
}
```
