---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d806c0cc5cd36d223b407d18ca7a0de3a60cea45
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774804"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}')
    .delete();

```