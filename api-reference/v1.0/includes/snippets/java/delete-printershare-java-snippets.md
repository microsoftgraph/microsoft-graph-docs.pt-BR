---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c33cb98ca0b58e06e43d40fa0badfed50cf5da1143eba3ff315d78070bb4d598
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100614"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{printerShareId}")
    .buildRequest()
    .delete();

```