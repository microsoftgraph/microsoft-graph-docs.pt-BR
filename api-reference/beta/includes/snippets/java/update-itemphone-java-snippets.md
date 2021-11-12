---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b15f560529a130d0bfa993f9da5cef5f5033afd6ba54fe0c8f572cf3c6194cca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899309"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPhone itemPhone = new ItemPhone();
itemPhone.type = PhoneType.OTHER;

graphClient.users("{userId}").profile().phones("{id}")
    .buildRequest()
    .patch(itemPhone);

```