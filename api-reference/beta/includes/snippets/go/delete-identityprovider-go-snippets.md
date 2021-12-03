---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 42195a21de4f9bf42306030478f2176c0cfc6bef
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286004"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityProviderId := "identityProvider-id"
graphClient.IdentityProvidersById(&identityProviderId).Delete(nil)


```