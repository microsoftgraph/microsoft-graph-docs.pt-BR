---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 711c18a2f8e0e1227c8d6e1f4bd8b6db25f4c709420c892d309727cad1e686b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100267"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/me/drive/items/{item-id}/content')
    .get();

```