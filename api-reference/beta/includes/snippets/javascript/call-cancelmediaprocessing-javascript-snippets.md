---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7a5d1e4ab7ca422c7e3f31177e9a2a7ee0b17fa37def75e05b8a26a4247a5d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271778"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancelMediaProcessingOperation = {
  clientContext: 'clientContext-value'
};

await client.api('/communications/calls/{id}/cancelMediaProcessing')
    .version('beta')
    .post(cancelMediaProcessingOperation);

```