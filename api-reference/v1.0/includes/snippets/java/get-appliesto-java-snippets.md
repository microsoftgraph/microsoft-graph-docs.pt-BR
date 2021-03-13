---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 116f4c1a14ea09a2d747153be8e4eea5068946f3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768825"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage appliesTo = graphClient.policies().claimsMappingPolicies("{id}").appliesTo()
    .buildRequest()
    .get();

```