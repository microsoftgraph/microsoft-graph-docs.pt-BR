---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ddc9ffb6a109f8e4cf169d3428af5e7f1ca7fe03d74938feb00fcf61c98c76c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101068"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRoleTemplates = await client.api('/directoryRoleTemplates')
    .get();

```