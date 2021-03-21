---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d64349fcbca804453ee8409dbf5f07531c5c239d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966647"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenIssuancePolicyCollectionWithReferencesPage tokenIssuancePolicies = graphClient.applications("{id}").tokenIssuancePolicies()
    .buildRequest()
    .get();

```