---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11039c485ad52f8d12e59ae759246b864c736697
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324635"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Identity().IdentityProviders().AvailableProviderTypes()().Get()


```