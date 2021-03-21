---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd4f39339925331043566f320eb9088cd046eb7e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969947"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage owners = graphClient.servicePrincipals("{id}").owners()
    .buildRequest()
    .get();

```