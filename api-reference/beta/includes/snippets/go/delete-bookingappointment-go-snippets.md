---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca0dd55312acff1950118c1b4cd8c5af9ad56be5
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286235"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingBusinessId := "bookingBusiness-id"
bookingAppointmentId := "bookingAppointment-id"
graphClient.BookingBusinessesById(&bookingBusinessId).AppointmentsById(&bookingAppointmentId).Delete(nil)


```