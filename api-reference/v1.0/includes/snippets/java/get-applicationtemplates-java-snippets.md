---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d766b12ceb92005362b004959f478d725b711a40
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970238"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApplicationTemplateCollectionPage applicationTemplates = graphClient.applicationTemplates()
    .buildRequest()
    .get();

```