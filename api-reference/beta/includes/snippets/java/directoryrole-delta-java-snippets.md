---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a74bde2943703752b17825e5b120ce1f1eb65c3b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976394"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRoleDeltaCollectionPage delta = graphClient.directoryRoles()
    .delta()
    .buildRequest()
    .get();

```