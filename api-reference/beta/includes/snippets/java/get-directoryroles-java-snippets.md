---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08f8a574a806a71d0e3e78a436d504ea16a06a14
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976930"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRoleCollectionPage directoryRoles = graphClient.directoryRoles()
    .buildRequest()
    .get();

```