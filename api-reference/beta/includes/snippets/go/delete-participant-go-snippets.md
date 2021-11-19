---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2ab6b1c7aa571bc55f27d35b7e0c235169e889a1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097969"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
participantId := "participant-id"
graphClient.Communications().CallsById(&callId).ParticipantsById(&participantId).Delete(options)


```