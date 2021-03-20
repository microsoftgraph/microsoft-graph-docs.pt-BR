---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28ff98681cab2280fe0f1a5c5838d816717e7ab9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976419"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationTemplateCollectionPage templates = graphClient.servicePrincipals("{id}").synchronization().templates()
    .buildRequest()
    .get();

```