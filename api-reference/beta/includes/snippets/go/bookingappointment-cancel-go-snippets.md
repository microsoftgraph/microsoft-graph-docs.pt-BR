---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: efe59bd72f0cbe2e5a6733d8381682a4875d18b9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091456"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
cancellationMessage := "Your appointment has been successfully cancelled. Please call us again."
requestBody.SetCancellationMessage(&cancellationMessage)
options := &msgraphsdk.CancelRequestBuilderPostOptions{
    Body: requestBody,
}
bookingBusinessId := "bookingBusiness-id"
bookingAppointmentId := "bookingAppointment-id"
graphClient.BookingBusinessesById(&bookingBusinessId).AppointmentsById(&bookingAppointmentId).Cancel().Post(options)


```