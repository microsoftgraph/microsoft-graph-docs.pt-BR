---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64df0a4ca8650b996a22a0d4be5e3eedc545bd10
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981319"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
itemPhoneId := "itemPhone-id"
graphClient.UsersById(&userId).Profile().PhonesById(&itemPhoneId).Delete(options)


```