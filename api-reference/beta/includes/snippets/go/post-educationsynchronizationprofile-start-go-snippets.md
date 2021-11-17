---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6fa44249f91ada6db7b9941cf998308351c666d9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018699"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationSynchronizationProfileId := "educationSynchronizationProfile-id"
result, err := graphClient.Education().SynchronizationProfilesById(&educationSynchronizationProfileId).Start().Post(options)


```