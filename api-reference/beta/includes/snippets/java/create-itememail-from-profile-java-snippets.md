---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7c47e2f9a30cef4ffc52e08c739ab30152652324
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969667"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemEmail itemEmail = new ItemEmail();
itemEmail.address = "Innocenty.Popov@adventureworks.com";

graphClient.me().profile().emails()
    .buildRequest()
    .post(itemEmail);

```