---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc6ee2802487b6c337eb91728ef77bfd3bf6f369
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981290"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

itemPhoneId := "itemPhone-id"
result, err := graphClient.Me().Profile().PhonesById(&itemPhoneId).Get(options)


```