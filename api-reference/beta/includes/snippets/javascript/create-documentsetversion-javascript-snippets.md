---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6757f0673c5cb53611de9e7d017a714f0e17ea34
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211488"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const documentSetVersion = {
  comment: 'v1',
  shouldCaptureMinorVersion: false
};

await client.api('/sites/root/lists/Documents/items/2/documentSetVersions')
    .version('beta')
    .post(documentSetVersion);

```