---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6ff8a3ad4d2fe0f2f2d98ccfd46b933f2fdc78538f0ae199d5cd2eb99b7433e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274743"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let list = await client.api('/sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))')
    .version('beta')
    .get();

```