---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f14cc6378d98d807b19af8329ee581c23b9df5bf8642dd610bff620cebbe2d2f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272093"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range')
    .version('beta')
    .get();

```