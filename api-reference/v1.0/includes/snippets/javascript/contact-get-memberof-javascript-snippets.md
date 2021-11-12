---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e823e19aba14302f13178238e200a55af227df6cdb35207e32148ac2aa37f55f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217063"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/contacts/{id}/memberOf')
    .get();

```