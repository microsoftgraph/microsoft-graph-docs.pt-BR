---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3554618d58ddd5a1ef3bc5fcb0e3a50ffec213ea82b3a165a07ccece32eb2de1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273606"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage owners = graphClient.servicePrincipals("{id}").owners()
    .buildRequest()
    .get();

```