---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d22dcbe22080b5d1ae930f99e6250800fb544478928b9b5f4b00515aa6dbde6f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275646"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var classes = await graphClient.Education.Me.Classes
    .Request()
    .GetAsync();

```