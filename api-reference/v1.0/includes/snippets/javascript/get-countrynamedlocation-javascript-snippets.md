---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b38c58655b3d8e29b929ed6ad07ff017176f7f4c51ff0802beb5abd406c99547
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101557"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let namedLocation = await client.api('/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959')
    .get();

```