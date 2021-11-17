---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 860f49cc5600ba4551bd025459d51af83d359bf8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60998021"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
itemEmailId := "itemEmail-id"
result, err := graphClient.UsersById(&userId).Profile().EmailsById(&itemEmailId).Get(options)


```