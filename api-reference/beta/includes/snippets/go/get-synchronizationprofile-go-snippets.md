---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bad52be2ba67421b13d9adc6d36b34bc5e6a77d7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091289"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationSynchronizationProfileId := "educationSynchronizationProfile-id"
graphClient.Education().SynchronizationProfilesById(&educationSynchronizationProfileId).Delete(options)


```