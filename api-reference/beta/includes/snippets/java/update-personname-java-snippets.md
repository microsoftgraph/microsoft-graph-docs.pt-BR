---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75eb54c8f92a6dd98cc00a7f80e1ac570f1c442a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971864"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonName personName = new PersonName();
personName.nickname = "Kesha";

graphClient.me().profile().names("{id}")
    .buildRequest()
    .patch(personName);

```