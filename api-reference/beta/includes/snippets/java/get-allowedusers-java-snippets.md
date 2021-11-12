---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1d4515a85e07980ac9239b55de5d89c0b04af89b45462468ea155bdea6421105
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899740"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserCollectionWithReferencesPage allowedUsers = graphClient.print().shares("{id}").allowedUsers()
    .buildRequest()
    .get();

```