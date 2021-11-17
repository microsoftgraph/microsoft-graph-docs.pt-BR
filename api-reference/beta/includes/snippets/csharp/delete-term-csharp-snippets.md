---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96d3695d9d96151768e6d91f0877823babef62540dc473e5498dac341e9beb85
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273206"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TermStore.Sets["{termStore.set-id}"].Terms["{termStore.term-id}"]
    .Request()
    .DeleteAsync();

```