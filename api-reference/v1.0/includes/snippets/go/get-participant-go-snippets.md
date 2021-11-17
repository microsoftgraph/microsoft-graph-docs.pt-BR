---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43775d2e39a545a34af2130e6c62a7e3e347e3cd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027268"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

callId := "call-id"
participantId := "participant-id"
result, err := graphClient.Communications().CallsById(&callId).ParticipantsById(&participantId).Get(options)


```