---
title: Tipo de recurso skypeForBusinessActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: a37cee0adbfaf64be649589a6493edc8eebf086b7f45b73bc51dc1cb9ae132d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54241321"
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
| isDeleted                                | Boolean           |
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


