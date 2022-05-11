---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2efb3ad9e6b3d62b3a9f98f3a3651e509a74b6d3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324360"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingBusinessId := "bookingBusiness-id"
bookingStaffMemberId := "bookingStaffMember-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).StaffMembersById(&bookingStaffMemberId).Get()


```