---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0a750ed2ddb9e7277aeb6e1db9174129c28cd25f1879f99e150b5a68b1af3e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329877"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSettings = await graphClient.GroupSettings
    .Request()
    .GetAsync();

```