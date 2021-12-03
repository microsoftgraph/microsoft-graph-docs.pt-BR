---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1d4cdf3fc990485324d10a1ddd5a5c59bebbeb6
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286516"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).Settings().ShiftPreferences().Get(nil)


```