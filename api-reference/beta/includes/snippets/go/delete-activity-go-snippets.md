---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d992b7630db8ecc3e6c84f894d0a26527941d786
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032134"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userActivityId := "userActivity-id"
graphClient.Me().ActivitiesById(&userActivityId).Delete(options)


```