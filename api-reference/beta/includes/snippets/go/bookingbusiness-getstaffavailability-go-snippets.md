---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47e5c4410093c83124f6ec0662e9de2476cf8086
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322907"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingBusinessId := "bookingBusiness-id"
graphClient.BookingBusinessesById(&bookingBusinessId).GetStaffAvailability(bookingBusiness-id).Get()


```