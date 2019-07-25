---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76ba8c499949b35135dcd2e73f213d7a115facb3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710480"
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