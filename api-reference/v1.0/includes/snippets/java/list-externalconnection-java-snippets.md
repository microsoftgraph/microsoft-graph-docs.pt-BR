---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 307c8f7557553ad56cd4aa30b6e4da53d2fe4881
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696818"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalConnectionCollectionPage connections = graphClient.external().connections()
    .buildRequest()
    .get();

```