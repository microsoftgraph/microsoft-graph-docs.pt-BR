---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29522765be4bbe5b7c35f46a2a0ffa7ca38f3f2c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740826"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var inferenceClassificationOverride = new InferenceClassificationOverride
{
    ClassifyAs = InferenceClassificationType.Focused,
    SenderEmailAddress = new EmailAddress
    {
        Name = "Samantha Booth",
        Address = "samanthab@adatum.onmicrosoft.com"
    }
};

await graphClient.Me.InferenceClassification.Overrides
    .Request()
    .AddAsync(inferenceClassificationOverride);

```