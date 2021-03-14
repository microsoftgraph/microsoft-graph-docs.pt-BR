---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7ad0814071f0981efcd3058ee9fb32a2bb1c2bf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796498"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/root/workbook/worksheets/{id}/range/rowsAbove')
    .get();

```