---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbd31fc7cdef157796d39f5ebb679332d191227d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322140"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().LicenseDetails().Get()


```