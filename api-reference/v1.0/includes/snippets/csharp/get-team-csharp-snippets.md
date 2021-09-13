---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4622149058ce24776bbe6274be143e64712b563ea4fb778cd433777685b918ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099289"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = await graphClient.Teams["{team-id}"]
    .Request()
    .GetAsync();

```