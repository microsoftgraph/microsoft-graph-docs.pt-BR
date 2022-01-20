---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec49316d51fe6d0af4c111f230c58de71d2b0b09
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095647"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.DeviceManagement().VirtualEndpoint().GetEffectivePermissions()().Get(nil)


```