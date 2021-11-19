---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1abe9085d26ba15fc9df9a1c5b7ea34b310282e4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101544"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingBusinessId := "bookingBusiness-id"
bookingCustomerId := "bookingCustomer-id"
graphClient.BookingBusinessesById(&bookingBusinessId).CustomersById(&bookingCustomerId).Delete(options)


```