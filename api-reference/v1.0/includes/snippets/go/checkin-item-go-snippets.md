---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b96d5a984eae338337c442adec0d42ed10b857d4
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094655"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
comment := "Updating the latest guidelines"
requestBody.SetComment(&comment)
driveId := "drive-id"
driveItemId := "driveItem-id"
graphClient.DrivesById(&driveId).ItemsById(&driveItemId).Checkin(drive-id, driveItem-id).Post(requestBody)


```