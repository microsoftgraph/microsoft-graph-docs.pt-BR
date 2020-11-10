---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1352d9aafe1a4bf7da60cfef5617ef5b4572c68f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955767"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.name = "My Day at the Beach";
driveItem.additionalDataManager().put("@microsoft.graph.conflictBehavior", new JsonPrimitive("rename"));
Bundle bundle = new Bundle();
Album album = new Album();
bundle.album = album;
driveItem.bundle = bundle;
LinkedList<DriveItem> childrenList = new LinkedList<DriveItem>();
DriveItem children = new DriveItem();
children.id = "1234asdf";
childrenList.add(children);
DriveItemCollectionResponse driveItemCollectionResponse = new DriveItemCollectionResponse();
driveItemCollectionResponse.value = childrenList;
DriveItemCollectionPage driveItemCollectionPage = new DriveItemCollectionPage(driveItemCollectionResponse, null);
driveItem.children = driveItemCollectionPage;

graphClient.drive().bundles()
    .buildRequest()
    .post(driveItem);

```