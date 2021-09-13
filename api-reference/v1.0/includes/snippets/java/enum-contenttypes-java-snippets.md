---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6ff82d40fd8390d76179ab0b3040f5314914ba0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026050"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContentTypeCollectionPage contentTypes = graphClient.sites("{site-id}").contentTypes()
    .buildRequest()
    .get();

```