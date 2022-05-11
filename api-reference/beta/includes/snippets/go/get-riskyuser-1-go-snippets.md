---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06301910178bb030759390fd60a14cb6db3f1e6e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324313"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

riskyUserId := "riskyUser-id"
result, err := graphClient.RiskyUsersById(&riskyUserId).Get()


```