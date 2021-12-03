---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6abe1070df5239678f3b37cc4a8717b2c517001
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285881"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Analytics().ActivityStatistics().Get(nil)


```