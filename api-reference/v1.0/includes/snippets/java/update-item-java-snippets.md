---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5716373ea8454b41e1f9a23fd11201456b47db62
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881605"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.name = "new-file-name.docx";

graphClient.me().drive().items("{item-id}")
    .buildRequest()
    .patch(driveItem);

```