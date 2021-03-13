---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e252e6e97047013c342839a517f2e99e5464f81c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774569"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personCertification = new PersonCertification
{
    IssuingAuthority = "International Academy of Marketing Excellence",
    IssuingCompany = "International Academy of Marketing Excellence"
};

await graphClient.Users["{user-id}"].Profile.Certifications["{personCertification-id}"]
    .Request()
    .UpdateAsync(personCertification);

```