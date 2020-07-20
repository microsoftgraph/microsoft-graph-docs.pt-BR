---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85d6c2419ccd456357080ae8ac6e03e5e6a11b2a
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791172"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var regionalAndLanguageSettings = await graphClient.Me.Settings.RegionalAndLanguageSettings
    .Request()
    .GetAsync();

```