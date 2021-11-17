---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75c586daad09973baa86fd97c01f87f7ae882f3e3498b36ac409b2be656dcdcb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271801"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languages = await graphClient.Me.Profile.Languages
    .Request()
    .GetAsync();

```