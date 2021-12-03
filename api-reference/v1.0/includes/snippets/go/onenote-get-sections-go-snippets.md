---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 094bac6c1c66e186de9263e25fbc15ca302716d7
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286604"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Onenote().Sections().Get(nil)


```