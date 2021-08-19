---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c9a3b5d0b09d8a6729491918f2039e99ade49aaea268e4dd24e2509477fa7df4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102349"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chats = await graphClient.Users["{user-id}"].Chats
    .Request()
    .Filter("members/any(o: o/displayname eq 'Peter Parker')")
    .Expand("members")
    .GetAsync();

```