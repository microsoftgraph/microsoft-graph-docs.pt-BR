---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9ebb76612eece02b84cb542eb3f9a83179108654a9427babbbca878ea600b950
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272300"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().authentication().phoneMethods("3179e48a-750b-4051-897c-87b9720928f7")
    .enableSmsSignIn()
    .buildRequest()
    .post();

```