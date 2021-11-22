---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81152651825f5b37c81d9069c001a12b1326fb6f4fd6eac5e584724bf4af0ea9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216257"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Authentication.WindowsHelloForBusinessMethods["{windowsHelloForBusinessAuthenticationMethod-id}"]
    .Request()
    .DeleteAsync();

```