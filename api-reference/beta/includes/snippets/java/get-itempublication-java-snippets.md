---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed8c21deef2bbfcf6e71a9ae121d76d06295d9e7f3a95cf69157c0e78c9d91fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329125"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPublication itemPublication = graphClient.me().profile().publications("{id}")
    .buildRequest()
    .get();

```