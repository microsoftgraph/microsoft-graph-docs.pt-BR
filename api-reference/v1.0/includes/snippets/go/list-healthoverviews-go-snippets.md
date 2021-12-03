---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: abc7ebc0e8ea5bf75d44ffd65ebb27db07329453
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287017"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Admin().ServiceAnnouncement().HealthOverviews().Get(nil)


```