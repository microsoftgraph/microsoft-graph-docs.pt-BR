---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 120a20146920338b1cdfd374e3b40ba701d70ecd16a8717f21c38c2d885f8d6f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213747"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personName = await graphClient.Me.Profile.Names["{personName-id}"]
    .Request()
    .GetAsync();

```