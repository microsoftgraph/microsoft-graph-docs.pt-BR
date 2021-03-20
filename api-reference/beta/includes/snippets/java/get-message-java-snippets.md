---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 437f8edf54c9cc774026e680a0164db8e356c29c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976663"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkAGI1AAAoZCfHAAA=")
    .buildRequest()
    .get();

```