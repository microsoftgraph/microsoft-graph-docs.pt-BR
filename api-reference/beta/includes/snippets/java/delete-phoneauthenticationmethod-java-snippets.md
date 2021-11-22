---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0573ab370a9c975f1750df574c8930c691d6c9b229f0b8fb15bee0cd9df056a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215158"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().authentication().phoneMethods("3179e48a-750b-4051-897c-87b9720928f7")
    .buildRequest()
    .delete();

```