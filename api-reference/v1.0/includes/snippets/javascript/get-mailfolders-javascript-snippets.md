---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 952cd7f2ddd2cc647305e60535726fdb01800f1c7e12cd28e7a1e6374a8b0ba1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899834"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mailFolders = await client.api('/me/mailFolders')
    .get();

```