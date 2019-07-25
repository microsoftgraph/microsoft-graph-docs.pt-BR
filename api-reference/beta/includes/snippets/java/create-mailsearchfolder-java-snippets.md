---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3e1bbbd157e666ee2adc9783b61e2d0bab42c803
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879855"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = new MailFolder();
mailFolder.additionalDataManager().put("@odata.type", new JsonPrimitive("microsoft.graph.mailSearchFolder"));
mailFolder.displayName = "Weekly digests";
mailFolder.includeNestedFolders = true;
LinkedList<String> sourceFolderIdsList = new LinkedList<String>();
sourceFolderIdsList.add("AQMkADYAAAIBDAAAAA==");
mailFolder.sourceFolderIds = sourceFolderIdsList;
mailFolder.filterQuery = "contains(subject, 'weekly digest')";

graphClient.me().mailFolders("AQMkADYAAAIBDAAAAA==").childFolders()
    .buildRequest()
    .post(mailFolder);

```