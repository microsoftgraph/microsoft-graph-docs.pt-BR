---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8f5d46da564e7fe7e6c662b450beeb523a98dadd26c2020a0b2775133faf4f8f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897868"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let alerts = await client.api('/security/alerts')
    .get();

```