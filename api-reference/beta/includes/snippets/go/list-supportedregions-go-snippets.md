---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9a7c27f78ae395cf4bbc2f0622d801d72d061e0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323189"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.DeviceManagement().VirtualEndpoint().SupportedRegions().Get()


```