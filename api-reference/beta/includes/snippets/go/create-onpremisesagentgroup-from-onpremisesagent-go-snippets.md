---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc4afe3d0aa61ad6f0cc3c66463b26a3d131118b
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285799"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
onPremisesAgentId := "onPremisesAgent-id"
onPremisesAgentGroupId := "onPremisesAgentGroup-id"
graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).AgentsById(&onPremisesAgentId).AgentGroupsById(&onPremisesAgentGroupId).Post(nil)


```