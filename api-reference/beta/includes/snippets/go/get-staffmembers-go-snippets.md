---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 295977966d4ebcc0b5f4c22f53ba0a728d39a6ef
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286228"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingBusinessId := "bookingBusiness-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).StaffMembers().Get(nil)


```