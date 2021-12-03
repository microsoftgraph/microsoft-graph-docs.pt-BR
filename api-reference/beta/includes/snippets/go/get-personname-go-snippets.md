---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67a5dddb447eed41bce932c20b28d00ef62090b6
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286247"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personNameId := "personName-id"
result, err := graphClient.Me().Profile().NamesById(&personNameId).Get(nil)


```