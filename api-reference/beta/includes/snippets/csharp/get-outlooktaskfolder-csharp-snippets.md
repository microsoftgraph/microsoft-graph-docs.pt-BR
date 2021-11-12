---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 476c56b0f425d529a00bddfe209690ea3050f47005ac15e289016c4ba28112cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160076"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskFolder = await graphClient.Me.Outlook.TaskFolders["{outlookTaskFolder-id}"]
    .Request()
    .GetAsync();

```