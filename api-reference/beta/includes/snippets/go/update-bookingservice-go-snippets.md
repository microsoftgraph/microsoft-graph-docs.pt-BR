---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64acaaf2964563369ac96a59b7b268743f188b91
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323368"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingService()
defaultDuration := "PT30M"
requestBody.SetDefaultDuration(&defaultDuration)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.bookingService",
}
bookingBusinessId := "bookingBusiness-id"
bookingServiceId := "bookingService-id"
graphClient.BookingBusinessesById(&bookingBusinessId).ServicesById(&bookingServiceId).Patch(requestBody)


```