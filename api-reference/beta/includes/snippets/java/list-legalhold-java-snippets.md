---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd70bcb3c6448669575a165afcbe9836a2a9e7be51a4c2ee59a7450d7c2ec629
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159687"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LegalHoldCollectionPage legalHolds = graphClient.compliance().ediscovery().cases("{caseId}").legalHolds()
    .buildRequest()
    .get();

```