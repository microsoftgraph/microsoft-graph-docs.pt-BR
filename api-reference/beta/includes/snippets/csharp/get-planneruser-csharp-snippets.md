---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81908466b4b9eea7488c595667872e89a77a1cc6cf0ee35e262a51cbd2b1eef4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159095"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerUser = await graphClient.Me.Planner
    .Request()
    .GetAsync();

```