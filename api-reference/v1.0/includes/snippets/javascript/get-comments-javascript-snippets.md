---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 049971537ce37adaf54a8aacac5ca8f6dafe6dbe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788406"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let comments = await client.api('/drive/items/{id}/workbook/comments')
    .get();

```