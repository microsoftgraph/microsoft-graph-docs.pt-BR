---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e79a9e2026ae30deb8d75f7c36f6beb8495707e7
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286215"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveItemId := "driveItem-id"
result, err := graphClient.Drive().BundlesById(&driveItemId).Get(nil)


```