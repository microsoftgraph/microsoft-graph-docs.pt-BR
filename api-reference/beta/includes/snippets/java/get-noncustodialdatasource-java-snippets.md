---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bced32f1d68ee6c8dbe8017b629e2eeb08626586
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240939"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NoncustodialDataSource noncustodialDataSource = graphClient.compliance().ediscovery().cases("5b840b94-f821-4c4a-8cad-3a90062bf51a").noncustodialDataSources("8b69818bf6af4f8a9dede428401c71e7")
    .buildRequest()
    .get();

```