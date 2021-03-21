---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49196681c86578a57c6920a01a0f7f8cb3a0c092
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982493"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectionOperation connectionOperation = graphClient.connections("contosohr").operations("3ed1595a-4bae-43c2-acda-ef973e581323")
    .buildRequest()
    .get();

```