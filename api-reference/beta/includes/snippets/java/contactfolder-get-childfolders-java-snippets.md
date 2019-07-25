---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7902d05724ec6a8924047ed39849e8896f326588
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863243"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IContactFolderCollectionPage childFolders = graphClient.me().contactFolders("{id}").childFolders()
    .buildRequest()
    .get();

```