---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76ba8c499949b35135dcd2e73f213d7a115facb3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517668"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = new Agreement
{
    DisplayName = "MSGraph Sample",
    IsViewingBeforeAcceptanceRequired = true,
    Files = new List<AgreementFile>()
    {
        new AgreementFile
        {
            FileName = "TOU.pdf",
            Language = "en",
            IsDefault = true,
            FileData = new AgreementFileData
            {
                Data = "SGVsbG8gd29ybGQ="
            }
        }
    }
};

await graphClient.Agreements
    .Request()
    .AddAsync(agreement);

```