---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e14eb8137d0712d47da05eba8f6717ced6cede40
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806632"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printConnector = await client.api('/print/connectors/{id}')
    .version('beta')
    .get();

```