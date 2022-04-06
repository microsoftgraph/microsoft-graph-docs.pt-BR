---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd8581384a4a11051e1b74d883daa210b3674c93
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516095"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreementFile = await graphClient.IdentityGovernance.TermsOfUse.Agreements["{agreement-id}"].File
    .Request()
    .GetAsync();

```