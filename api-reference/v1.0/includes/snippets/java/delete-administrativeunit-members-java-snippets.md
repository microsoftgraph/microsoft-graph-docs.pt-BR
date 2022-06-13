---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c40f8de62c5891a08240c1431552cca4a0d27184
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040867"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().administrativeUnits("{id1}").members("{id2}").reference()
    .buildRequest()
    .delete();

```