---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72367e186825af5862bdfe3cc0de8ad16aaab281
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040913"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionPage members = graphClient.directory().administrativeUnits("{id}").members().references()
    .buildRequest()
    .get();

```