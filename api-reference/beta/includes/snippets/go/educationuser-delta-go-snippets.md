---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 632fe50c53e48d0041f75ed6ee1b7317e74be938
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324679"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Education().Users().Delta()().Get()


```