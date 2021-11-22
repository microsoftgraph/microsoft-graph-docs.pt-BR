---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c53bd581714b0417c399665ded518781e74fa9ff9d0dad4101e6ff11ef36c77e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214686"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("061b9a92-8926-4bd9-b41d-abf35edc7583")
    .buildRequest()
    .delete();

```