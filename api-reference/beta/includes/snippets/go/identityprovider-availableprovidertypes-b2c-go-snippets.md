---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7271aedeb178d246b57938f5d57ed81720aa1179
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137602"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Identity().IdentityProviders().AvailableProviderTypes()().Get(nil)


```