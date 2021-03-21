---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9ce9ce7325ad7448ebb55adb68b7139bbc8314f7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983032"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADhMGAAA=")
    .buildRequest()
    .get();

```