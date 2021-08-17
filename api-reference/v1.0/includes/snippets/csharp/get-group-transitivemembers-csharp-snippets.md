---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 125d6ea1823dfe4ad8182b633618de010f9afdeef75311d997ee9e7897745c09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215104"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMembers = await graphClient.Groups["{group-id}"].TransitiveMembers
    .Request()
    .GetAsync();

```