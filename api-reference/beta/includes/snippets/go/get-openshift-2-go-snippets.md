---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8eac6d1b99bc57f1df1084f40567bc59ea6349d7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002852"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OpenShifts().Get(options)


```