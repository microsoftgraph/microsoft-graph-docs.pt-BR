---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77495a6d02cb9b045982384cfae081368e5383b8
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286637"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).Authentication().WindowsHelloForBusinessMethods().Get(nil)


```