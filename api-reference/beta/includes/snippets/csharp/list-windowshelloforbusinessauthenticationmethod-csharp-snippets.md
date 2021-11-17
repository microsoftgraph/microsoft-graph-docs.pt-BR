---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85c0bcd4a9cf88887b891666cb593cd63b4c24836e40c82f9e2fd5eed820bcd1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160145"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var windowsHelloForBusinessMethods = await graphClient.Users["{user-id}"].Authentication.WindowsHelloForBusinessMethods
    .Request()
    .GetAsync();

```