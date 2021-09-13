---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7c6aa09ac1a58d19341a7f387e34f44dc58de2a169d67cbadb1e757704c14a85
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/users/{idOrUserPrincipalName}/drive')
    .get();

```