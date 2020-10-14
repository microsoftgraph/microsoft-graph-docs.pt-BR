---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac4a3acc4144b8fbb3117747d048692cca77881f
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462454"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Subscriptions["7f105c7d-2dc5-4530-97cd-4e7ae6534c07"]
    .Request()
    .DeleteAsync();

```