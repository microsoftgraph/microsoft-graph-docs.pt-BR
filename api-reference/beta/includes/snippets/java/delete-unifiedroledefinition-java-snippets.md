---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f295aa32e14726b95dcfaccee1577157a2e7d0c5bd83371325b44fceb949ec8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274854"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.roleManagement().directory().roleDefinitions("f189965f-f560-4c59-9101-933d4c87a91a")
    .buildRequest()
    .delete();

```