---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1a5df000bea5f34981d8e514f640e98b280b1e1b9c2985135f30f4694217da05
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272222"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let recent = await client.api('/me/drive/recent')
    .get();

```