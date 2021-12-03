---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 624f8ce7cc1892f6f70f43479422d5f1c91e56d8
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286218"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingBusinessId := "bookingBusiness-id"
bookingStaffMemberId := "bookingStaffMember-id"
graphClient.BookingBusinessesById(&bookingBusinessId).StaffMembersById(&bookingStaffMemberId).Delete(nil)


```