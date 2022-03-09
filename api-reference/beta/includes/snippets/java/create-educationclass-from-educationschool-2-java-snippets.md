---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eba688b3d8d1be0ed5fa61241b11615c975537c7b8fd8e022a86b48ceeb24dce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215072"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("{id}").teachers("14012")
    .buildRequest()
    .delete();

```