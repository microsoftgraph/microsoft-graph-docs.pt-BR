---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9780623c713d8aedc8d37ca8c7b00ba034746795d40a935b8c438648916c449d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275071"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRoles = await client.api('/directoryRoles')
    .version('beta')
    .get();

```