---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4b2143aab9c0e4652bb23ea2c6b6c08f1be759a9
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287010"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

itemAddressId := "itemAddress-id"
result, err := graphClient.Me().Profile().AddressesById(&itemAddressId).Get(nil)


```