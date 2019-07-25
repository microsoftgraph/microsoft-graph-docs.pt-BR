---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3c556718b886662ba41471970cbf703445266b4a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713343"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles')
    .version('beta')
    .get();

```