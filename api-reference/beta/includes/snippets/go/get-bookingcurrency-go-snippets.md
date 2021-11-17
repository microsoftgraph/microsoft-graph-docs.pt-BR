---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f04ddc5e508fecc8ac17001807c4a1ee79fe036f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994730"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

bookingCurrencyId := "bookingCurrency-id"
result, err := graphClient.BookingCurrenciesById(&bookingCurrencyId).Get(options)


```