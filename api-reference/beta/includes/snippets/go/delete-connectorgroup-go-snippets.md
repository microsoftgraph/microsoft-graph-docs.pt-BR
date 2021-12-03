---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2f9dff860306b03d3c5a5159318beb74250edbdb
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286127"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
connectorGroupId := "connectorGroup-id"
graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).ConnectorGroupsById(&connectorGroupId).Delete(nil)


```