---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2de81667b5ed0cafe2f064c3cae0533de1d4fac9b389adedcd803ae49595d81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var photos = await graphClient.Groups["{group-id}"].Photos
    .Request()
    .GetAsync();

```