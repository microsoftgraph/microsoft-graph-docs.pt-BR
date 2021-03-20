---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4305c057a77e08decfd4abded659d07ed99411de
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978590"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Conversation conversation = graphClient.groups("{id}").conversations("{id}")
    .buildRequest()
    .get();

```