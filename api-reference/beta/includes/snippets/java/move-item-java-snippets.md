---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 472c8faaed6dbdc199d3d3498704539ba0656cba
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860988"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
ItemReference parentReference = new ItemReference();
parentReference.id = "new-parent-folder-id";
driveItem.parentReference = parentReference;
driveItem.name = "new-item-name.txt";

graphClient.me().drive().items("{item-id}")
    .buildRequest()
    .patch(driveItem);

```