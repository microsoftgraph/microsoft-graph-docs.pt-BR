---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c69190197b4bb58a8e2135bc5f7778ba5e9fe5ba
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977317"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.groups("b320ee12-b1cd-4cca-b648-a437be61c5cd")
    .buildRequest()
    .get();

```