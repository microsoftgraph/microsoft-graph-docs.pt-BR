---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 570e41443a2b739d9ea98464c0591ca0ec1121d927a29144c98fceb571131fd6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permission = await client.api('/me/drive/items/{item-id}/permissions/{perm-id}')
    .get();

```