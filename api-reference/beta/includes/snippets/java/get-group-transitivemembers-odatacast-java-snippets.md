---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85073e65dfada77cf9ca17c97abcb9967d12e8133f2e6ab2520bdc569f90343a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214836"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

GroupCollectionPage group = graphClient.groups("{id}").transitiveMembers().microsoft.graph.group()
    .buildRequest( requestOptions )
    .get();

```