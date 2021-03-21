---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9498a7e5e10607f5a6259a2f70358c8d14ba7d0c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984236"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationMethodCollectionPage methods = graphClient.me().authentication().methods()
    .buildRequest()
    .get();

```