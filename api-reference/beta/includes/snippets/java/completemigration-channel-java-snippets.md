---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0be5851010f68afb56808152567616509c1ce85
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508766"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("57fb72d0-d811-46f4-8947-305e6072eaa5").channels("19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2")
    .completeMigration()
    .buildRequest()
    .post();

```