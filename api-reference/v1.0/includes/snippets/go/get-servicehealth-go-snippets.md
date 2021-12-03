---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da5fd330474ff08bf6a59b9db36f1270fafe882e
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287123"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

serviceHealthId := "serviceHealth-id"
result, err := graphClient.Admin().ServiceAnnouncement().HealthOverviewsById(&serviceHealthId).Get(nil)


```