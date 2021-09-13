---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd0d54fb03fb5495b85188892d6509454e5ab88baac851eaa786d28e6608c98d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327541"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = new EducationClass
{
    Description = "History - World History 1",
    DisplayName = "World History Level 1"
};

await graphClient.Education.Classes["{educationClass-id}"]
    .Request()
    .UpdateAsync(educationClass);

```