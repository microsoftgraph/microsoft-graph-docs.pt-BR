---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60f5775740a84f36f48323c86e899fcddeb929173b1659f6f279ca6bfe9c8433
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275308"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let items = await client.api('/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)')
    .get();

```