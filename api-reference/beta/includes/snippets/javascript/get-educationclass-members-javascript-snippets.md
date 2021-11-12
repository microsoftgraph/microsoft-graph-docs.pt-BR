---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 931c08010c1d2c7484e8ef0202a63ea4e55842663828adc99e034896eba43c3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102430"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/education/classes/11016/members')
    .version('beta')
    .get();

```