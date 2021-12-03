---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb42a765e8d7e86ad1c12948a4c83a64cfc58a87
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286840"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().LicenseDetails().Get(nil)


```