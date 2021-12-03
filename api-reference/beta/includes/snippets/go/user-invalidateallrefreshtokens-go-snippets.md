---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61752f085d3f2c4a7d1f96d865d11f4de39482e9
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286861"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().InvalidateAllRefreshTokens().Post(nil)


```