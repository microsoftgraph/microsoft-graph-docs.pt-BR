---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 534e5b5d415423191477da02dca224c25142e578
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029278"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

secureScoreControlProfileId := "secureScoreControlProfile-id"
result, err := graphClient.Security().SecureScoreControlProfilesById(&secureScoreControlProfileId).Get(options)


```