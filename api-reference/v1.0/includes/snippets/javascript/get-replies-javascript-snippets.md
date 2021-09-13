---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed3e87ebc423aaed1b0ccdc9bc833f1350b53614f8e464cd258a58df6892833f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217036"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let replies = await client.api('/drive/items/{id}/workbook/comments/{id}/replies')
    .get();

```