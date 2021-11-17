---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e928039f79665aa92d80daf5d3a3850a652bda3f1338a9225d3ce029175f3e01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157269"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/users/{userId}/drives')
    .version('beta')
    .get();

```