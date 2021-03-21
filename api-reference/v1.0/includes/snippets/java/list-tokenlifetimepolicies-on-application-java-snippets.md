---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62b8a0c825ddca00bc0b2183c9ce11865b916b64
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983327"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenLifetimePolicyCollectionWithReferencesPage tokenLifetimePolicies = graphClient.applications("{id}").tokenLifetimePolicies()
    .buildRequest()
    .get();

```