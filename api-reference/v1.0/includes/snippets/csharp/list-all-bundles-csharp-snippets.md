---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a6e8308ce4d3b3022ce52a747c71942d0986003
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757880"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bundles = await graphClient.Drive.Bundles
    .Request()
    .GetAsync();

```