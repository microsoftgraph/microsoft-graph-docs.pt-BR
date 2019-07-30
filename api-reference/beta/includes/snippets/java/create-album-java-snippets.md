---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43da307a6ab14ae310d0c34a205abd07e5df8134
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932627"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.name = "My Day at the Beach";
driveItem.@name.conflictBehavior = "rename";
Bundle bundle = new Bundle();
Album album = new Album();
bundle.album = album;
driveItem.bundle = bundle;
LinkedList<DriveItem> childrenList = new LinkedList<DriveItem>();
DriveItem children = new DriveItem();
children.id = "1234asdf";
childrenList.add(children);
driveItem.children = childrenList;

graphClient.drive().bundles()
    .buildRequest()
    .post(driveItem);

```