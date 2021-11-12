---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8d7e925c30f6afe8a50c1f0679c99d9575f2f58833e634178001b2d46d530541
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215564"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskFolder outlookTaskFolder = graphClient.me().outlook().taskFolders("AAMkADIyAAAAABrJAAA=")
    .buildRequest()
    .get();

```