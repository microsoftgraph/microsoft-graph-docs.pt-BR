---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af6466538e1ea7436b2911e6e987700cea8c5624
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287304"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().CreatedObjects().Get(nil)


```