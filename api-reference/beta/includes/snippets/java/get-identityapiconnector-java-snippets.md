---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f339326f6e30976ab1125b3167101c205f873fde
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968989"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = graphClient.identity().apiConnectors("{id}")
    .buildRequest()
    .get();

```