---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7f079adeedc739cbbd96f7db21195a2179a3d53e0affce2ad0c8ac678fd6f08
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327038"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sectionGroups = await client.api('/me/onenote/sectionGroups/{id}/sectionGroups')
    .get();

```