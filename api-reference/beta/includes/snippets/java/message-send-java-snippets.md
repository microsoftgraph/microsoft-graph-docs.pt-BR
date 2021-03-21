---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0a8e9aa564b87b4458553b2f4f3df7bf69ea7de3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981602"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .send()
    .buildRequest()
    .post();

```