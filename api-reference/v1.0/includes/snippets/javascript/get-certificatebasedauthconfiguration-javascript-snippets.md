---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 008150eb34046a5578f5d7e55402a1806fee076a28b17890038b183eb9a13eea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272927"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let certificateBasedAuthConfiguration = await client.api('/organization/{id}/certificateBasedAuthConfiguration/{id}')
    .get();

```