---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4b6de07038877a2331aa1090bf7912866bc3ecfee82df69ff0f81d1dec8bdc6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329374"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var me = await graphClient.Me
    .Request()
    .Select("Responsibilities")
    .GetAsync();

var responsibilities = me.Responsibilities;

```