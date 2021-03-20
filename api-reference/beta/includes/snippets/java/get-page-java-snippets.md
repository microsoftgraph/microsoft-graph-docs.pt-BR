---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8804117edac43fa5b9e5c0bf71eb8b0645cac2a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968695"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SitePage sitePage = graphClient.sites("{site-id}").pages("{page-id}")
    .buildRequest()
    .get();

```