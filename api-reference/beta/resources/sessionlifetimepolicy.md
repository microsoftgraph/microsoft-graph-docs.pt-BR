---
title: Tipo de recurso sessionlifetimepolicy
description: Descreve as políticas de tempo de vida da sessão que o Azure AD aplicou a um evento de login.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 9da2ea66c726d48fa3b0a34c168debd16dbd8713
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137240"
---
# <a name="sessionlifetimepolicy-resource-type"></a>Tipo de recurso sessionlifetimepolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve as políticas de tempo de vida da sessão que o Azure AD aplicou a um evento de login. 

Para obter mais detalhes sobre o gerenciamento de sessão com acesso condicional no Azure AD, consulte a documentação de gerenciamento de sessão de acesso [condicional.](/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|expirationRequirement|expirationRequirement|Se uma política de gerenciamento de sessão de acesso condicional exigia que o usuário se autenticasse nesse evento de entrada, este campo descreveria o tipo de política que exigia autenticação. Os valores possíveis são `rememberMultifactorAuthenticationOnTrustedDevices`, `tenantTokenLifetimePolicy`, `audienceTokenLifetimePolicy`, `signInFrequencyPeriodicReauthentication`, `ngcMfa`, `signInFrequencyEveryTime`, `unknownFutureValue`.|
|detail|Cadeia de caracteres|Os detalhes de leitura humana da política de gerenciamento de sessão de acesso condicional aplicada à entrada.|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sessionLifetimePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sessionLifetimePolicy",
  "expirationRequirement": "String",
  "detail": "String"
}
```

