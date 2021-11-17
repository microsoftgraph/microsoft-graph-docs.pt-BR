---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b45318019696c4956ee4e5bcbed6e5a444625a4de6b6b6e536ac72704dbce55d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329617"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directReports = await client.api('/me/directReports')
    .version('beta')
    .get();

```