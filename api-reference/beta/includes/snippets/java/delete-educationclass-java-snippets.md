---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6311b9080fcd873c2ab57d6800ec4853931726a6e9bb467f2714d4d5e8bc8cb0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216378"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11022")
    .buildRequest()
    .delete();

```