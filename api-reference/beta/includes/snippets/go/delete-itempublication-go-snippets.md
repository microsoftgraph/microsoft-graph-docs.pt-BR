---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 170450cd6253c82e3fb35738b029b7a8b0588959
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286679"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

itemPublicationId := "itemPublication-id"
graphClient.Me().Profile().PublicationsById(&itemPublicationId).Delete(nil)


```