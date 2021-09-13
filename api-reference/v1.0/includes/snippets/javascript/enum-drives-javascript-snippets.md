---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17b02fdcffb2653605164d670726c9c16c17be57099bdfad06ccb997f3ccb349
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102718"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/me/drives')
    .get();

```