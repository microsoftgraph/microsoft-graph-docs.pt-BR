---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f7bcaee3db7e17674ba664dfd3f31400e41d8c4c83bbf10da3cc1d866b216f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214566"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("kim@contoso.com").authentication().emailMethods("3ddfcfc8-9383-446f-83cc-3ab9be4be18f")
    .buildRequest()
    .delete();

```