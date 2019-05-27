---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 452ed92d2ebedeb4fce3af43b4363e5da1e9be82
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434431"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingStaffMember = new BookingStaffMember
{
    ColorIndex = 1,
    DisplayName = "Dana Swope",
    EmailAddress = "danas@contoso.com",
    Role = BookingStaffRole.ExternalGuest,
    UseBusinessHours = true,
    WorkingHours = new List<BookingWorkHours>()
    {
        new BookingWorkHours
        {
            Day = DayOfWeek.Monday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = "17:00:00.0000000",
                    Start = "08:00:00.0000000"
                }
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Tuesday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = "17:00:00.0000000",
                    Start = "08:00:00.0000000"
                }
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Wednesday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = "17:00:00.0000000",
                    Start = "08:00:00.0000000"
                }
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Thursday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = "17:00:00.0000000",
                    Start = "08:00:00.0000000"
                }
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Friday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = "17:00:00.0000000",
                    Start = "08:00:00.0000000"
                }
            }
        }
    }
};

await graphClient.BookingBusinesses["{id}"].StaffMembers
    .Request()
    .AddAsync(bookingStaffMember);

```