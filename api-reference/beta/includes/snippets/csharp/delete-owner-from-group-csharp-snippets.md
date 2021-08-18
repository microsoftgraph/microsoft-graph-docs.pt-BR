---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be56a00a90daca592bf70a6afce3c97d5475efd223880b6e1472d496fcc5c978
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272567"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].Owners["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```