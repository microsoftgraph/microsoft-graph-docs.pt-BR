---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e29011cae6c610b16cf87926bfc2e4dad4e1d019b7590c8b4a9e04fa8e228715
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329657"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentCollectionPage roleAssignments = graphClient.roleManagement().directory().roleAssignments()
    .buildRequest()
    .get();

```