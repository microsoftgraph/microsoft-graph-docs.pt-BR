---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3d5a9b2159b4faf0a58cc4daf042ecc8972e30a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285943"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Education().Me().Assignments().Get(nil)


```