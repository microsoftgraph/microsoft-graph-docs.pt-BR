---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2aa125e349ad989a971b0656221e5d7738db5c0
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210694"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContractCollectionPage contracts = graphClient.contracts()
    .buildRequest()
    .get();

```