---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 303d6226d5462d47f49a1fd2c37a99562a49ea6d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975290"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CaseCollectionPage cases = graphClient.compliance().ediscovery().cases()
    .buildRequest()
    .get();

```