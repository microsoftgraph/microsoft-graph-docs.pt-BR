---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9eabbc259cc750604b9359deee4df25e0bb40e2c8c19a8dddb34e40ff1ecc9d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272783"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{item-id}')
    .delete();

```