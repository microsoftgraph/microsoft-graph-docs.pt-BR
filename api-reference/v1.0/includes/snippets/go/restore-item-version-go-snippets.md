---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 727501f4708a36e7bbddc20a42ee275f84e1b07a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324773"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveId := "drive-id"
driveItemId := "driveItem-id"
driveItemVersionId := "driveItemVersion-id"
graphClient.DrivesById(&driveId).ItemsById(&driveItemId).VersionsById(&driveItemVersionId).RestoreVersion(drive-id, driveItem-id, driveItemVersion-id).Post()


```