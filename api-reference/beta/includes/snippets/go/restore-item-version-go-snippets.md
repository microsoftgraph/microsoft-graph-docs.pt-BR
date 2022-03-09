---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d56d06c525b9dbfcd983cba9311f43f18000df59
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395073"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveId := "drive-id"
driveItemId := "driveItem-id"
driveItemVersionId := "driveItemVersion-id"
graphClient.DrivesById(&driveId).ItemsById(&driveItemId).VersionsById(&driveItemVersionId).RestoreVersion(drive-id, driveItem-id, driveItemVersion-id).Post(nil)


```