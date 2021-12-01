---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45f8884b07b0a7c1b28bd59799d44bf86f685584d14822903390eb53ab94d914
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103116"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permission = new Permission
{
    Roles = new List<String>()
    {
        "read"
    }
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Permissions["{permission-id}"]
    .Request()
    .UpdateAsync(permission);

```