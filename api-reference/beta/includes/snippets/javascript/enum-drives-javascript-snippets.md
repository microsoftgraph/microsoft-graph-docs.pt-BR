---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c42f64e444766c7ceabeedd59f65aca7c18380195cb1fd95e2a5e907acd7a09f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100846"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/me/drives')
    .version('beta')
    .get();

```