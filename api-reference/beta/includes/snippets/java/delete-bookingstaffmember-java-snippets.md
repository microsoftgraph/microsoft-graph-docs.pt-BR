---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2e6b3ee7bf3f8109cb5964c7da6de3981fea36a0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977454"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").staffMembers("5fae928f-6d2d-417a-ad96-4b0caeb362d6")
    .buildRequest()
    .delete();

```