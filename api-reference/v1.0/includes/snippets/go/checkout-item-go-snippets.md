---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c658ca1cd464d734a7db6bbb3b2a57b841fd4905
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093259"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveId := "drive-id"
driveItemId := "driveItem-id"
graphClient.DrivesById(&driveId).ItemsById(&driveItemId).Checkout(drive-id, driveItem-id).Post()


```