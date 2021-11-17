---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47126e287a8ec1ba2f40329c758da8a24deb67944b5f7fa0017ac39ccd450df7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156747"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let languageProficiency = await client.api('/me/profile/languages/{id}')
    .version('beta')
    .get();

```