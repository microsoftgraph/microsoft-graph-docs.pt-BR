---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: daa9e31b891cb586dd954084decb7bc134246893
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092101"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
participantId := "participant-id"
result, err := graphClient.Communications().CallsById(&callId).ParticipantsById(&participantId).Get(options)


```