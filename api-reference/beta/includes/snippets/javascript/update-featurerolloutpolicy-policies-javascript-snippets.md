---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8219cd0567eab8168e31ba71696777051157adf9f614effb5e3c87878e510308
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157758"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const featureRolloutPolicy = {
  displayName: 'PasswordHashSync Rollout Policy',
  description: 'PasswordHashSync Rollout Policy',
  isEnabled: true,
  isAppliedToOrganization: false
};

await client.api('/policies/featureRolloutPolicies/d7ab4886-d7f0-441b-a5e6-e62d7328d18a')
    .version('beta')
    .update(featureRolloutPolicy);

```