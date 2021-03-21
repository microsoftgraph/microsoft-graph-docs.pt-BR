---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e02a452f95ef807ceb4465b82d619592d08e127b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969576"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

StringCollectionPage responsibilities = graphClient.customRequest("/me/responsibilities", StringCollectionPage.class)
    .buildRequest()
    .get();

```