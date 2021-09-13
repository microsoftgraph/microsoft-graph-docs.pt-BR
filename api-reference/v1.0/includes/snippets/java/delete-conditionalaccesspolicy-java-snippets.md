---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 103c3d6812b14a2a4825f444ec55669b9a8116f9e6d5a07b26c551c0d424b2ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216520"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().conditionalAccess().policies("{id}")
    .buildRequest()
    .delete();

```