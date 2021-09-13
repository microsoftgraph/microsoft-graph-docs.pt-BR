---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06df857d9fd79a877b5fe0438eb183a153687deeec6f1e81d0b26a115c34583e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406712"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkingHours workingHours = graphClient.customRequest("/me/mailboxSettings/workingHours", WorkingHours.class)
    .buildRequest()
    .get();

```