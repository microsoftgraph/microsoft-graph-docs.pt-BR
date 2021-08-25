---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b99011c5efdaa08fba4696a393e507ab51161f1fa442c82abab517332f2d90b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327937"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.termStore().groups("{groupId}")
    .buildRequest()
    .delete();

```