---
title: tipo de recurso Presence
description: Contém informações sobre a presença de um usuário, incluindo a disponibilidade e a atividade do usuário.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 48574baf0969077add921d6b4c9d52dd2d5d4906
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913566"
---
# <a name="presence-resource-type"></a>tipo de recurso Presence

Contém informações sobre a presença de um usuário, incluindo a disponibilidade e a atividade do usuário.

> **Observação:** No momento, esse recurso só tem suporte para usuários do Microsoft Teams.

## <a name="methods"></a>Methods

| Método                                                            | Tipo de retorno                                       | Descrição                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [Obter presença](../api/presence-get.md)     | [presença](../resources/presence.md)     | Obtenha as informações de presença de um usuário.
| [Obter presença de vários usuários](../api/cloudcommunications-getpresencesbyuserid.md)    |  coleção [Presence](../resources/presence.md)     |  Obtenha as informações de presença de vários usuários.      |


## <a name="properties"></a>Propriedades

| Relação        | Tipo                                                 | Descrição                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|id    |  cadeia de caracteres     |  A ID de objeto de usuário   |
|availability    |  coleção de cadeias de caracteres   |   As informações de presença básicas de um usuário. Os valores possíveis `Available`são `AvailableIdle`, `Away`, `BeRightBack` `Busy` `BusyIdle`,,, `DoNotDisturb`, `Offline`,,`PresenceUnknown`  |
|atividade    |  coleção de cadeias de caracteres      |    As informações complementares para a disponibilidade de um usuário. Os valores possíveis `Available`são `Away`, `BeRightBack``Busy` `DoNotDisturb` `InACall`,,,, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.       |

>**Observação:** Para saber mais sobre os diferentes Estados de presença, confira [presença do usuário no Microsoft Teams](https://docs.microsoft.com/microsoftteams/presence-admins). 

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.presence"
}-->
```json
{
   "id":"string",
   "availability":"string",
   "activity":"string"
}
```
