---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa025e209cbd5c851aef96bf596c606a1a2eae4a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968957"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemEmail itemEmail = new ItemEmail();
itemEmail.displayName = "Business Email";
itemEmail.type = EmailType.WORK;

graphClient.users("{userId}").profile().emails("{id}")
    .buildRequest()
    .patch(itemEmail);

```