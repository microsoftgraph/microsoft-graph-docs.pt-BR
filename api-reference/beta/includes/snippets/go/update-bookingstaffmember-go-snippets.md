---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8fce76c73fccc4890d7591d34b3e14aad068c61d
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094246"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingStaffMember()
requestBody.SetWorkingHours( []BookingWorkHours {
    msgraphsdk.NewBookingWorkHours(),
day := "monday"
    SetDay(&day)
    SetTimeSlots( []BookingWorkTimeSlot {
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.bookingWorkHours",
        "day@odata.type": "#microsoft.graph.dayOfWeek",
        "timeSlots@odata.type": "#Collection(microsoft.graph.bookingWorkTimeSlot)",
    }
    msgraphsdk.NewBookingWorkHours(),
day := "tuesday"
    SetDay(&day)
    SetTimeSlots( []BookingWorkTimeSlot {
        msgraphsdk.NewBookingWorkTimeSlot(),
end := "17:00:00.0000000"
        SetEnd(&end)
start := "08:00:00.0000000"
        SetStart(&start)
        SetAdditionalData(map[string]interface{}{
            "@odata.type": "#microsoft.graph.bookingWorkTimeSlot",
        }
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.bookingWorkHours",
        "day@odata.type": "#microsoft.graph.dayOfWeek",
        "timeSlots@odata.type": "#Collection(microsoft.graph.bookingWorkTimeSlot)",
    }
    msgraphsdk.NewBookingWorkHours(),
day := "wednesday"
    SetDay(&day)
    SetTimeSlots( []BookingWorkTimeSlot {
        msgraphsdk.NewBookingWorkTimeSlot(),
end := "17:00:00.0000000"
        SetEnd(&end)
start := "08:00:00.0000000"
        SetStart(&start)
        SetAdditionalData(map[string]interface{}{
            "@odata.type": "#microsoft.graph.bookingWorkTimeSlot",
        }
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.bookingWorkHours",
        "day@odata.type": "#microsoft.graph.dayOfWeek",
        "timeSlots@odata.type": "#Collection(microsoft.graph.bookingWorkTimeSlot)",
    }
    msgraphsdk.NewBookingWorkHours(),
day := "thursday"
    SetDay(&day)
    SetTimeSlots( []BookingWorkTimeSlot {
        msgraphsdk.NewBookingWorkTimeSlot(),
end := "17:00:00.0000000"
        SetEnd(&end)
start := "08:00:00.0000000"
        SetStart(&start)
        SetAdditionalData(map[string]interface{}{
            "@odata.type": "#microsoft.graph.bookingWorkTimeSlot",
        }
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.bookingWorkHours",
        "day@odata.type": "#microsoft.graph.dayOfWeek",
        "timeSlots@odata.type": "#Collection(microsoft.graph.bookingWorkTimeSlot)",
    }
    msgraphsdk.NewBookingWorkHours(),
day := "friday"
    SetDay(&day)
    SetTimeSlots( []BookingWorkTimeSlot {
        msgraphsdk.NewBookingWorkTimeSlot(),
end := "17:00:00.0000000"
        SetEnd(&end)
start := "08:00:00.0000000"
        SetStart(&start)
        SetAdditionalData(map[string]interface{}{
            "@odata.type": "#microsoft.graph.bookingWorkTimeSlot",
        }
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.bookingWorkHours",
        "day@odata.type": "#microsoft.graph.dayOfWeek",
        "timeSlots@odata.type": "#Collection(microsoft.graph.bookingWorkTimeSlot)",
    }
}
bookingBusinessId := "bookingBusiness-id"
bookingStaffMemberId := "bookingStaffMember-id"
graphClient.BookingBusinessesById(&bookingBusinessId).StaffMembersById(&bookingStaffMemberId).Patch(requestBody)


```