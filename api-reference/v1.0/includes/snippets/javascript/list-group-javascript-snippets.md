---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dac24b5e87a2a75f40065c43cf26b4a1ea2e7ebf5b42861e4f326e65cee7bbcf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101012"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let allowedGroups = await client.api('/print/shares/{printerShareId}/allowedGroups')
    .get();

```