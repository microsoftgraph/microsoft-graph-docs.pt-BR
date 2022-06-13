---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82bf170235d7289c60fd836ef436993699db7ab6
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "66040983"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.IdentityProviders().AvailableProviderTypes()().Get()


```