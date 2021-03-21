---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 043cf31fcc9f01d46298ee65ceb7853234c7134c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980245"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPhone itemPhone = new ItemPhone();
itemPhone.displayName = "Car Phone";
itemPhone.number = "+7 499 342 22 13";

graphClient.me().profile().phones()
    .buildRequest()
    .post(itemPhone);

```