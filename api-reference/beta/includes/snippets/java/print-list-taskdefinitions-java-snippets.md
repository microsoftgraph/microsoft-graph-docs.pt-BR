---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 056efb8c6ba8f8974d0e2d3c769b682b47c6f52e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978917"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskDefinitionCollectionPage taskDefinitions = graphClient.print().taskDefinitions()
    .buildRequest()
    .get();

```