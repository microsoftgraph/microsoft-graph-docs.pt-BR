---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 005956f37d265946d648e4bcaccc266fd697ddd3
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240791"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NoncustodialDataSourceCollectionWithReferencesPage noncustodialSources = graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("{sourceCollectionId}").noncustodialSources()
    .buildRequest()
    .get();

```