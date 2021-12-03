---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71788cc287bbd1d04ec266b60f89cb24f6f3dbfe
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286005"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Authentication().Fido2Methods().Get(nil)


```