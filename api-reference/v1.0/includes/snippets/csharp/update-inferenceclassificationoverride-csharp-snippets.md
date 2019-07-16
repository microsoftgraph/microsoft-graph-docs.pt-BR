---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01852563a2e17275dfee2155b3124408772940cf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738916"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var inferenceClassificationOverride = new InferenceClassificationOverride
{
    ClassifyAs = InferenceClassificationType.Focused
};

await graphClient.Me.InferenceClassification.Overrides["{id}"]
    .Request()
    .UpdateAsync(inferenceClassificationOverride);

```