---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5e05f1dbf9213a04104e652a5a53957562656cd9ce7691d5b4f1cbd774ff7c91
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329664"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var projects = await graphClient.Me.Profile.Projects
    .Request()
    .GetAsync();

```