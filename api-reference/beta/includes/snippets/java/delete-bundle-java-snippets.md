---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9518f231b8dfef144c457d45a8105072c6ff9c5a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978103"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().items("{bundle-id}")
    .buildRequest()
    .delete();

```