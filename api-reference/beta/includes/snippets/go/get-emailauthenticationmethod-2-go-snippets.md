---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 910210394061b35baddaa4ebc9d42fa8b9188e4d
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287194"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Authentication().EmailMethods().Get(nil)


```