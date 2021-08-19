---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 644adb0883b6e9aab9d61997855dae47f03bb3d553abd8554b90738f1f85a77f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272891"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Me.Contacts
    .Request()
    .GetAsync();

```