---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba858b1d88d4044065b1c793f92f266ac55c2d72
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61006471"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Drive().Get(options)


```