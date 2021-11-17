---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 501a020e3d0f6800023ab2f7c09df5b32d6f5c33
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981354"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

itemPatentId := "itemPatent-id"
result, err := graphClient.Me().Profile().PatentsById(&itemPatentId).Get(options)


```