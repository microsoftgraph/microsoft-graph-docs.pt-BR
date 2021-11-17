---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8491666af91e5467ea8d1dd922082e378aca3b74f732f984ec75b98e0847ba51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159136"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let siteSource = await client.api('/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources/38304445-3741-3333-4233-344238454333')
    .version('beta')
    .get();

```