---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4292a091bd7e9c2effc2afe8b991f7331c3e103
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285769"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Education().Me().Schools().Get(nil)


```