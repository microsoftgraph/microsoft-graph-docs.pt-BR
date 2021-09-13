---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3011e3eeaa11e1fe8d166a994eeed4c6cfdc30a91d05dc1c7ffd4a290c2f7018
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327128"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rubrics = await client.api('/education/me/rubrics')
    .get();

```