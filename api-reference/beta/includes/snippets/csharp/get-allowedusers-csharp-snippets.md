---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00eb1e0a8c7678ec05d966e99b3072bad78ddc951ddb262f21bcda1414de9715
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102268"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var allowedUsers = await graphClient.Print.Shares["{printerShare-id}"].AllowedUsers
    .Request()
    .GetAsync();

```