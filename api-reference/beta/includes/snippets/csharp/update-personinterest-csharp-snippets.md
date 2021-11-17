---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72fd561cf0147c226bdd48f95a3db984eac08d30084e8c1d13aeeeb4bc44b72c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156457"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personInterest = new PersonInterest
{
    Categories = new List<String>()
    {
        "Sports"
    }
};

await graphClient.Me.Profile.Interests["{personInterest-id}"]
    .Request()
    .UpdateAsync(personInterest);

```