---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 05cf17dc1db735f76bc29ca2a4893206eef7bcbb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978758"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Alert alert = graphClient.security().alerts("{id}")
    .buildRequest()
    .get();

```