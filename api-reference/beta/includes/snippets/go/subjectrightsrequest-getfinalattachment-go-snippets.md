---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67b155a16f86e766173a5ef28a0d0fdbad5e11ef
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719121"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

subjectRightsRequestId := "subjectRightsRequest-id"
graphClient.Privacy().SubjectRightsRequestsById(&subjectRightsRequestId).GetFinalAttachment()(subjectRightsRequest-id).Get()


```