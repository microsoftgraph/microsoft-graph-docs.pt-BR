---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88ee8484b504e466ad91a08ffde9bf3872105939
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981253"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage owners = graphClient.groups("{id}").owners()
    .buildRequest()
    .get();

```