---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28218355dfbbfc253311a730ef4c9a622c0eeccb4f8dec070419b6e0d404b3eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103029"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"]
    .Request()
    .DeleteAsync();

```