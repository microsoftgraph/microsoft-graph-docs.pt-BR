---
title: tipo de recurso skypeForBusinessActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 28b57aa0a6cb1f7684c26f3cf60ed531534f76a4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997554"
---
# <a name="skypeforbusinessactivityuserdetail-resource-type"></a>tipo de recurso skypeForBusinessActivityUserDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade                                 | Tipo              |
| :--------------------------------------- | :---------------- |
| totalPeerToPeerSessionCount              | Int64             |
| totalOrganizedConferenceCount            | Int64             |
| totalParticipatedConferenceCount         | Int64             |
| peerToPeerLastActivityDate               | Data              |
| organizedConferenceLastActivityDate      | Data              |
| participatedConferenceLastActivityDate   | Data              |
| peerToPeerIMCount                        | Int64             |
| peerToPeerAudioCount                     | Int64             |
| peerToPeerAudioMinutes                   | Int64             |
| peerToPeerVideoCount                     | Int64             |
| peerToPeerVideoMinutes                   | Int64             |
| peerToPeerAppSharingCount                | Int64             |
| peerToPeerFileTransferCount              | Int64             |
| organizedConferenceIMCount               | Int64             |
| organizedConferenceAudioVideoCount       | Int64             |
| organizedConferenceAudioVideoMinutes     | Int64             |
| organizedConferenceAppSharingCount       | Int64             |
| organizedConferenceWebCount              | Int64             |
| organizedConferenceDialInOut3rdPartyCount | Int64             |
| organizedConferenceCloudDialInOutMicrosoftCount | Int64             |
| organizedConferenceCloudDialInMicrosoftMinutes | Int64             |
| organizedConferenceCloudDialOutMicrosoftMinutes | Int64             |
| participatedConferenceIMCount           | Int64             |
| participatedConferenceAudioVideoCount   | Int64             |
| participatedConferenceAudioVideoMinutes | Int64             |
| participatedConferenceAppSharingCount   | Int64             |
| participatedConferenceWebCount          | Int64             |
| participatedConferenceDialInOut3rdPartyCount | Int64             |
| reportRefreshDate                        | Data              |
| userPrincipalName                        | String            |
| isDeleted                                | Boolean           |
| deletedDate                              | Data              |
| lastActivityDate                         | Data              |
| assignedProducts                         | Coleção de cadeias de caracteres |
| reportPeriod                             | String            |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserDetail"
} -->

```json
{
  "totalPeerToPeerSessionCount": 1024,
  "totalOrganizedConferenceCount": 1024,
  "totalParticipatedConferenceCount": 1024,
  "peerToPeerLastActivityDate": "Date",
  "organizedConferenceLastActivityDate": "Date",
  "participatedConferenceLastActivityDate": "Date",
  "peerToPeerIMCount": 1024,
  "peerToPeerAudioCount": 1024,
  "peerToPeerAudioMinutes": 1024,
  "peerToPeerVideoCount": 1024,
  "peerToPeerVideoMinutes": 1024,
  "peerToPeerAppSharingCount": 1024,
  "peerToPeerFileTransferCount": 1024,
  "organizedConferenceIMCount": 1024,
  "organizedConferenceAudioVideoCount": 1024,
  "organizedConferenceAudioVideoMinutes": 1024,
  "organizedConferenceAppSharingCount": 1024,
  "organizedConferenceWebCount": 1024,
  "organizedConferenceDialInOut3rdPartyCount": 1024,
  "organizedConferenceCloudDialInOutMicrosoftCount": 1024,
  "organizedConferenceCloudDialInMicrosoftMinutes": 1024,
  "organizedConferenceCloudDialOutMicrosoftMinutes": 1024,
  "participatedConferenceIMCount": 1024,
  "participatedConferenceAudioVideoCount": 1024,
  "participatedConferenceAudioVideoMinutes": 1024,
  "participatedConferenceAppSharingCount": 1024,
  "participatedConferenceWebCount": 1024,
  "participatedConferenceDialInOut3rdPartyCount": 1024,
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "isDeleted": true,
  "deletedDate": "Date",
  "lastActivityDate": "Date",
  "assignedProducts": ["String"],
  "reportPeriod": "String"
}
```


