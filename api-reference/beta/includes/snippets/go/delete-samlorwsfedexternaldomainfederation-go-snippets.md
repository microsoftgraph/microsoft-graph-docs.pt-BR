---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bebcc483c77c0c75e4e4529c48a3ab1525cf3014
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285858"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityProviderBaseId := "identityProviderBase-id"
graphClient.Directory().FederationConfigurationsById(&identityProviderBaseId).Delete(nil)


```