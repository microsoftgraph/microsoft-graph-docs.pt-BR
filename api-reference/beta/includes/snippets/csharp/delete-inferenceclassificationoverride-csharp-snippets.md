---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d268b25c3cadc718d647eb031701ca37fe2116172b170e23678416382406c329
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216037"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.InferenceClassification.Overrides["{inferenceClassificationOverride-id}"]
    .Request()
    .DeleteAsync();

```