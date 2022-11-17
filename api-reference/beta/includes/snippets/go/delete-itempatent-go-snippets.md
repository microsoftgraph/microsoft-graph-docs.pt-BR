---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0f3709568b6f92ccc4007136c43d8b28917c203d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020772"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
itemPatentId := "itemPatent-id"
graphClient.UsersById(&userId).Profile().PatentsById(&itemPatentId).Delete(options)


```