---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da45895b0ef633702cedd2e8d243442a03bb023a5f1434cb6dc54a0811bd7866
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102719"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Users["{user-id}"].Drives
    .Request()
    .GetAsync();

```