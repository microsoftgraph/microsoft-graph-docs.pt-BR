---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c245faeecef8dbd310f88a0807239d76b340b528
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100751"
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
options := &msgraphsdk.BookingBusinessRequestBuilderPatchOptions{
    Body: requestBody,
}
bookingBusinessId := "bookingBusiness-id"
graphClient.BookingBusinessesById(&bookingBusinessId).Patch(options)


```