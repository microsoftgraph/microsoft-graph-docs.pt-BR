---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3123ba2a4ff5c9fe4b3e7072ae41db3581c07bbb7fd5507f5db99d60f2218cde
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215353"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Outlook.TaskGroups["{outlookTaskGroup-id}"]
    .Request()
    .DeleteAsync();

```