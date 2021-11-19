---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac5aff4294253e86ee23dd862dc7261e38337fa1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096110"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingBusinessId := "bookingBusiness-id"
bookingCustomerId := "bookingCustomer-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).CustomersById(&bookingCustomerId).Get(options)


```