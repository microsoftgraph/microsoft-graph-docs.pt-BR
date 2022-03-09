---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4f4a5ff37236eba38589263666f2031e28c7130
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393280"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

riskyUserId := "riskyUser-id"
result, err := graphClient.IdentityProtection().RiskyUsersById(&riskyUserId).History().Get(nil)


```