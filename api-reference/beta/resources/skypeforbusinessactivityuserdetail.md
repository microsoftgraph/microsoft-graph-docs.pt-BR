---
title: Tipo de recurso skypeForBusinessActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 48067fa9b6a4b64262cc5f7c374d5513451de74b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068421"
---
# <a name="skypeforbusinessactivityuserdetail-resource-type"></a>Tipo de recurso skypeForBusinessActivityUserDetail

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
| userPrincipalName                        | Cadeia de caracteres            |
| isDeleted                                | Booliano           |
| deletedDate                              | Data              |
| lastActivityDate                         | Data              |
| assignedProducts                         | String collection |
| reportPeriod                             | Cadeia de caracteres            |

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


