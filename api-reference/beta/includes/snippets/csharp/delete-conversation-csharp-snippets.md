---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e33a3d451813a50a3d96cd305051dc45fca2ed9a5cd4afeb77e5e84dc7590525
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216985"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].Conversations["{conversation-id}"]
    .Request()
    .DeleteAsync();

```