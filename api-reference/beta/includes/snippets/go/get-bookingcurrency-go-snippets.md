---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0033eb09a660671c251ed310b0437721e4723d71
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324435"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingCurrencyId := "bookingCurrency-id"
result, err := graphClient.BookingCurrenciesById(&bookingCurrencyId).Get()


```