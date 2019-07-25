---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa0bc3e12aa9f83df4af63b56bfde06b5cd5c5e7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894813"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/installedApps')
    .expand('teamsAppDefinition')
    .get();

```