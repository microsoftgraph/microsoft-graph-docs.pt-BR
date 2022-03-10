---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0e70a182fa2bbb8447bebe1b71a4709b75096d59
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410638"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingBusinessId := "bookingBusiness-id"
bookingCustomQuestionId := "bookingCustomQuestion-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).CustomQuestionsById(&bookingCustomQuestionId).Delete(nil)


```