---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9816086116a03b3a3f060a84a8c5fa533b1bd08
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798406"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsAppInstallation = await client.api('/teams/{id}/installedApps/{id}')
    .expand('teamsAppDefinition')
    .get();

```