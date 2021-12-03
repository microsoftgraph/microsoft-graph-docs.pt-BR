---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 16ce32e56c66aeb6679eb4261b515332c10c76d1
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286125"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
connectorGroupId := "connectorGroup-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).ConnectorGroupsById(&connectorGroupId).Get(nil)


```