---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91f94d40a2ff303f474ecf2e6fa131895da4ebe8
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287435"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Profile().Languages().Get(nil)


```