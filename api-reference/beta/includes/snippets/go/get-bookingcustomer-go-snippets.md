---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5e21046b129a7e097744b2df64285c48a58b86f2
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286221"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingBusinessId := "bookingBusiness-id"
bookingCustomerId := "bookingCustomer-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).CustomersById(&bookingCustomerId).Get(nil)


```