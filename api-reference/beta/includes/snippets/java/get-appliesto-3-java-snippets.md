---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9d7d15f849a8cef61f86b350ad137c04e46d117
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962742"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage appliesTo = graphClient.policies().tokenIssuancePolicies("{id}").appliesTo()
    .buildRequest()
    .get();

```