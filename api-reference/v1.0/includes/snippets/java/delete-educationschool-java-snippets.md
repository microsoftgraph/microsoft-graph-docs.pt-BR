---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b060a2916c55a308197b79f8eeb65f401f304c9ce68059f1debb4092b1527ebc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326853"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("{school-id}")
    .buildRequest()
    .delete();

```