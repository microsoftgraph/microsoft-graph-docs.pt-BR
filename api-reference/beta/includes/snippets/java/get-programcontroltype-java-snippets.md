---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4c508f3026a954d3b493a125e2ff21a56cd56b0d44ac26375958c2fdaaa7ede6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217155"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProgramControlTypeCollectionPage programControlTypes = graphClient.programControlTypes()
    .buildRequest()
    .get();

```