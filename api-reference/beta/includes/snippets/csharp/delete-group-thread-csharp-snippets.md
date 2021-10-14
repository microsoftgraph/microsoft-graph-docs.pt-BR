---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1bdb7ff4cc03191f308e8d57ad97d6dfacd1ead08ed3e1dd67fc00f2ae9d523
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156496"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"]
    .Request()
    .DeleteAsync();

```