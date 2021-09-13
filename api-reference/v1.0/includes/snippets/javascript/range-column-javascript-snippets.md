---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2552df1f6de989d67718451e6fd1beee79fb1c2237fde0a6cc7768e81d0ef4bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100232"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)')
    .get();

```