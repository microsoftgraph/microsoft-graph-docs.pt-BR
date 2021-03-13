---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2a3e990fe39120f44f4a8ab50a92859240c7b217
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776505"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SourceCollection sourceCollection = new SourceCollection();
sourceCollection.displayName = "Quarterly Financials search";

graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("1a9b4145d8f84e39bc45a7f68c5c5119")
    .buildRequest()
    .patch(sourceCollection);

```