---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ac52e8439bddb9d5020d35300fccfaa43101738
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605952"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookSessionInfo = {
  persistChanges: true
};

let res = await client.api('/me/drive/items/{id}/workbook/createSession')
    .post(workbookSessionInfo);

```