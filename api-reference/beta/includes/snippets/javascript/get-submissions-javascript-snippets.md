---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 456fe7e7bbb3cb79c764710e85267c77189bd166
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472167"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let submissions = await client.api('/education/classes/11021/assignments/19002/submissions')
    .version('beta')
    .get();

```