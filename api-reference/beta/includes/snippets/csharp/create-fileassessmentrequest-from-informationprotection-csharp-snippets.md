---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31f8c292694d3456836317f68dc0a775a68c15fdf5836a0ab62b310ccf18f5cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156954"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = new FileAssessmentRequestObject
{
    ExpectedAssessment = ThreatExpectedAssessment.Block,
    Category = ThreatCategory.Malware,
    FileName = "test.txt",
    ContentData = "VGhpcyBpcyBhIHRlc3QgZmlsZQ=="
};

await graphClient.InformationProtection.ThreatAssessmentRequests
    .Request()
    .AddAsync(threatAssessmentRequest);

```