---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b44e6fb5e8f5fda63eac80e118b3f0fa878a9706
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024405"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeOffReasons().Get(options)


```