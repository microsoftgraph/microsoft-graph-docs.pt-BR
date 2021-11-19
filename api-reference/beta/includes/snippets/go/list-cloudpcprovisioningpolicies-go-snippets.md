---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc8e9fd554015cb5fa9188a17ac5f0485e16d12d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092839"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.DeviceManagement().VirtualEndpoint().ProvisioningPolicies().Get(options)


```