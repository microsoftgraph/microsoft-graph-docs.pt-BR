---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6037836929c1a39c2dc5158f3cbd51d8edf4249e
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286388"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

externalConnectionId := "externalConnection-id"
graphClient.External().ConnectionsById(&externalConnectionId).Delete(nil)


```