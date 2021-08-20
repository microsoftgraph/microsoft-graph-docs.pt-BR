---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7868371fc71dfc0a7a873e39ac8c81217f7520efe55156babfcb106314d6f386
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159978"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var resources = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Resources
    .Request()
    .GetAsync();

```