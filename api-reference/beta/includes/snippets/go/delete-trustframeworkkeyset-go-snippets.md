---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b084bce2ceef1572608f14bfa4f9136c491b8151
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286783"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

trustFrameworkKeySetId := "trustFrameworkKeySet-id"
graphClient.TrustFramework().KeySetsById(&trustFrameworkKeySetId).Delete(nil)


```