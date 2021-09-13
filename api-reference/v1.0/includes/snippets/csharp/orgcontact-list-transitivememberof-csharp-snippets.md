---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 078bc90b5a9edb9da7ec4c297e482dce4b8159f44cb0a67951370ca28e0da113
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329697"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.Contacts["{orgContact-id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```