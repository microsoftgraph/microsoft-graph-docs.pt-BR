---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2acb983d5a2ecd2916f1b77274df29ff8411db4e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974232"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionPage groups = graphClient.groups()
    .buildRequest()
    .filter("membershipRuleProcessingState eq 'On'")
    .select("id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus")
    .get();

```