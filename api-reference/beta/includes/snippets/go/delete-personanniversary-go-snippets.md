---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b327d7b8b849678bd047f79cd7684be145bc62a8
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287449"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personAnnualEventId := "personAnnualEvent-id"
graphClient.Me().Profile().AnniversariesById(&personAnnualEventId).Delete(nil)


```