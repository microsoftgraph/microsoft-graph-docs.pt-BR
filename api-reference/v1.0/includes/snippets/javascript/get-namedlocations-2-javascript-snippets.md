---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 279b167d8726bd186ad44c1b0ddb882e333e3c18306090b1da775b757f3021cb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215309"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let namedLocations = await client.api('/identity/conditionalAccess/namedLocations')
    .filter('isof(\'microsoft.graph.ipNamedLocation\')')
    .get();

```