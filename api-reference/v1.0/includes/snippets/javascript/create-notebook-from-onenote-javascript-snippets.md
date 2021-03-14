---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d79b96352a224f0a940f44abad7a38922b3093f5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778668"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const notebook = {
  displayName: 'Notebook name'
};

await client.api('/me/onenote/notebooks')
    .post(notebook);

```