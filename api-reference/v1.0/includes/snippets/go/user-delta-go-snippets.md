---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 183fe3cf82e386142fca7a1ac4e35a7a18b6b52e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315137"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Users().Delta()().Get()


```