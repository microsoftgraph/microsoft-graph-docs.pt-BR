---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aebaccf8b8a13198fbdf85422a0713d02e18ab54ae82b88a2c3985f1f950529e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406925"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:Web"));

ApplicationCollectionPage applications = graphClient.applications()
    .buildRequest( requestOptions )
    .get();

```