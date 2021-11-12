---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2f644a74ac7667d8d3d33996bebc5e9a99f6f7495db7823a4af22c348d132df6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215348"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskFolders = await graphClient.Me.Outlook.TaskFolders
    .Request()
    .GetAsync();

```