---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97ae300b3d7112cbf60494276cb00395995b29c9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805789"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)')
    .get();

```