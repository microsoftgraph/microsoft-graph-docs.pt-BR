---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f555e7cadda13fab6e15d79b0d0894a27cb70185a2da8aaf8e3f9bc016504a07
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273097"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeOffReason = {
  displayName: 'Vacation',
  iconType: 'plane',
  isActive: true
};

await client.api('/teams/{teamId}/schedule/timeOffReasons')
    .post(timeOffReason);

```