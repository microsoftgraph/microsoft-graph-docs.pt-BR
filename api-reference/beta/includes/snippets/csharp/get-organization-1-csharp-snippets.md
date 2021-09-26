---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a48f380782cee50e22c2b39843da294e1da4911b1f2a2429c743102f558edbef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275103"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organization = await graphClient.Organization
    .Request()
    .GetAsync();

```