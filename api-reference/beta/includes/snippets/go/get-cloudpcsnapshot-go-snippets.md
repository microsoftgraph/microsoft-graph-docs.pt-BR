---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97d1a09475a22f89684ce6da94017284f3cd0f27
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323911"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcSnapshotId := "cloudPcSnapshot-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().SnapshotsById(&cloudPcSnapshotId).Get()


```