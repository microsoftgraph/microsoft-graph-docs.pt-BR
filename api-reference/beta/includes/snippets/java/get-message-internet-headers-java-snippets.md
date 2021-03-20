---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 681a679ed126e13fe6d316271d08d804b4eac800
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972490"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkAGVmMDEz")
    .buildRequest()
    .select("internetMessageHeaders")
    .get();

```