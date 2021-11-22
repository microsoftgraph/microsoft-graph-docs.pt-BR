---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c141d9bcbfda57328f862ee9545ef4083ee4979c0be31cdfb2aaf0ec50541355
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159587"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.trustFramework().keySets("{id}")
    .buildRequest()
    .delete();

```