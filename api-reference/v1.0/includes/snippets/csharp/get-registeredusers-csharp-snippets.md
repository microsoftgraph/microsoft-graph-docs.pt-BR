---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b963dc8851832a1387bfb0a5a6d75e521149488e6d4e715da6ad1a8f076d49c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216517"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var registeredUsers = await graphClient.Devices["{device-id}"].RegisteredUsers
    .Request()
    .GetAsync();

```