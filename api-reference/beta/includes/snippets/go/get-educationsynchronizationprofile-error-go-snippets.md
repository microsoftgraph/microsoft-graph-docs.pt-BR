---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4d84e7d60860478e73ed9658a76cf78e15f68cc6
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286687"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationSynchronizationProfileId := "educationSynchronizationProfile-id"
result, err := graphClient.Education().SynchronizationProfilesById(&educationSynchronizationProfileId).Errors().Get(nil)


```