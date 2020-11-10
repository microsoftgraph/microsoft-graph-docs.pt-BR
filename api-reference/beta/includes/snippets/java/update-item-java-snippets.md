---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5716373ea8454b41e1f9a23fd11201456b47db62
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964162"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.name = "new-file-name.docx";

graphClient.me().drive().items("{item-id}")
    .buildRequest()
    .patch(driveItem);

```