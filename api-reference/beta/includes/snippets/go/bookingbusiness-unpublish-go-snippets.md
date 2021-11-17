---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb1864f2d28cbbe958585e2b910a039a98098dee
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994751"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

bookingBusinessId := "bookingBusiness-id"
graphClient.BookingBusinessesById(&bookingBusinessId).Unpublish().Post(options)


```