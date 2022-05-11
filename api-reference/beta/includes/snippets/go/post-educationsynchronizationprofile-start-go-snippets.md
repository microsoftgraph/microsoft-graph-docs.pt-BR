---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2a8ade02d637d4b1c2b8f94fdcc7a32735ad120
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323229"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationSynchronizationProfileId := "educationSynchronizationProfile-id"
result, err := graphClient.Education().SynchronizationProfilesById(&educationSynchronizationProfileId).Start(educationSynchronizationProfile-id).Post()


```