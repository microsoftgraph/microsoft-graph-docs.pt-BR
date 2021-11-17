---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dce40b722378c98a4fd0ec276b88d96acee741fa
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021976"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

onlineMeetingId := "onlineMeeting-id"
meetingRegistrationQuestionId := "meetingRegistrationQuestion-id"
result, err := graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().CustomQuestionsById(&meetingRegistrationQuestionId).Get(options)


```