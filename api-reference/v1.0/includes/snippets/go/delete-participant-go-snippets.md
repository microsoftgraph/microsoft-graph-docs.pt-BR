---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 320dc136fb32673f197d4ff2d0e35bfd5ebe7c96
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322756"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
participantId := "participant-id"
graphClient.Communications().CallsById(&callId).ParticipantsById(&participantId).Delete()


```