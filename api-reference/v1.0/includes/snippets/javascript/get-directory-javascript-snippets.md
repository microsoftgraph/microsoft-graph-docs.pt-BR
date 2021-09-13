---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b802d468b096cc612e8e7bf1c030e51e5dec6fc208a16022d18a19ee7fca0cb7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57330058"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/directory/deletedItems/{object-id}')
    .get();

```