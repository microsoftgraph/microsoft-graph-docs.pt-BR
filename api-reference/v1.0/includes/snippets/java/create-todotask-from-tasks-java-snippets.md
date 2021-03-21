---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9802ea6e3feb11cd39caf09ab8f9ff7f022bbe5d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980481"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTask todoTask = new TodoTask();
todoTask.title = "A new task";
LinkedList<LinkedResource> linkedResourcesList = new LinkedList<LinkedResource>();
LinkedResource linkedResources = new LinkedResource();
linkedResources.webUrl = "http://microsoft.com";
linkedResources.applicationName = "Microsoft";
linkedResources.displayName = "Microsoft";
linkedResourcesList.add(linkedResources);
LinkedResourceCollectionResponse linkedResourceCollectionResponse = new LinkedResourceCollectionResponse();
linkedResourceCollectionResponse.value = linkedResourcesList;
LinkedResourceCollectionPage linkedResourceCollectionPage = new LinkedResourceCollectionPage(linkedResourceCollectionResponse, null);
todoTask.linkedResources = linkedResourceCollectionPage;

graphClient.me().todo().lists("AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM").tasks()
    .buildRequest()
    .post(todoTask);

```