---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4ce75d9e2c4a468e4463c8094f44a2813f36e52c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324603"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingBusiness()
email := "admin@fabrikam.com"
requestBody.SetEmail(&email)
schedulingPolicy := msgraphsdk.NewBookingSchedulingPolicy()
requestBody.SetSchedulingPolicy(schedulingPolicy)
timeSlotInterval := "PT60M"
schedulingPolicy.SetTimeSlotInterval(&timeSlotInterval)
minimumLeadTime := "P1D"
schedulingPolicy.SetMinimumLeadTime(&minimumLeadTime)
maximumAdvance := "P30D"
schedulingPolicy.SetMaximumAdvance(&maximumAdvance)
sendConfirmationsToOwner := true
schedulingPolicy.SetSendConfirmationsToOwner(&sendConfirmationsToOwner)
allowStaffSelection := true
schedulingPolicy.SetAllowStaffSelection(&allowStaffSelection)
bookingBusinessId := "bookingBusiness-id"
graphClient.BookingBusinessesById(&bookingBusinessId).Patch(requestBody)


```