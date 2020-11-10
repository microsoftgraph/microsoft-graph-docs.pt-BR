---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1daab45af5355536081877ea709ede8c63bc24d2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954470"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("kim@contoso.com").authentication().fido2Methods("_jpuR-TGZtk6aQCLF3BQjA2")
    .buildRequest()
    .delete();

```