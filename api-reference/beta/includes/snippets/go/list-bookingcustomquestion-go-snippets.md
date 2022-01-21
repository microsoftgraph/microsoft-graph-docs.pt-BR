---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28006f39a85da0c0f97c1c8b78a469c993e8ae04
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114026"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingBusinessId := "bookingBusiness-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).CustomQuestions().Get(nil)


```