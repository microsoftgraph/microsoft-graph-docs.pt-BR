---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbfc32a2ab75b53a0f374d247639888217e6765c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982465"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPC cloudPC = graphClient.deviceManagement().virtualEndpoint().cloudPCs("{id}")
    .buildRequest()
    .get();

```