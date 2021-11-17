---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 581a85ec352b6f64d11cc42ccc230e862a318241
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022004"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
onlineMeetingId := "onlineMeeting-id"
meetingRegistrantId := "meetingRegistrant-id"
graphClient.UsersById(&userId).OnlineMeetingsById(&onlineMeetingId).Registration().RegistrantsById(&meetingRegistrantId).Delete(options)


```