---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b9f847134c24e4d881e405e0b562c5a65bfc6dd2ac9742eb7c4bf8a300b86bf2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100426"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedApproval = await graphClient.PrivilegedApproval["{privilegedApproval-id}"]
    .Request()
    .GetAsync();

```