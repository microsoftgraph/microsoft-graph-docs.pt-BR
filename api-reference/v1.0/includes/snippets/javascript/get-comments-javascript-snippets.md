---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fce295d7a94cb04f9868ddb50c685213933c0fdd
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46512142"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/items/{id}/workbook/comments')
    .get();

```