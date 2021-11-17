---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54243b2928545c25e699c6845047964d074f410a38b7ae8c43e35f8489ead9e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271832"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().mailFolders("AAMkAGVmMDEzM")
    .buildRequest()
    .delete();

```