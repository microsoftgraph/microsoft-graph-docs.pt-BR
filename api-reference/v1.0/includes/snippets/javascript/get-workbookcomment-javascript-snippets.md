---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbaa38d89fcec014faffd45d3e4113e9fe66ebad
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781995"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookComment = await client.api('/drive/items/{id}/workbook/comments/{id}')
    .get();

```