---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 693852789b8d3502c40dd130290e68562d733b4c2f2fd13f853cdae2cd9dcdd8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272860"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sourceCollections = await client.api('/compliance/ediscovery/cases/{caseId}/sourceCollections')
    .version('beta')
    .get();

```