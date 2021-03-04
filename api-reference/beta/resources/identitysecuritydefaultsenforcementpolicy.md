---
title: Tipo de recurso identitySecurityDefaultsEnforcementPolicy
description: Representa a política de padrões de segurança do Azure Active Directory. Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.
localization_priority: Normal
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b06fd0b88a87dabb5a12e09b788094b8e00b8960
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440250"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a>Tipo de recurso identitySecurityDefaultsEnforcementPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a política de padrões de [segurança](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) do Azure Active Directory. Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.

Herda de [policyBase](../resources/policybase.md).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | Leia as propriedades de **um objeto identitySecurityDefaultsEnforcementPolicy.** |
| [Atualização](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | Atualize **um objeto identitySecurityDefaultsEnforcementPolicy.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String|Descrição dessa política. Somente leitura.|
|displayName|String|Nome de exibição para esta política. Somente leitura.|
|id|String|Identificador dessa política. Somente leitura.|
|isEnabled|Booliano|Se definido como true, os padrões de segurança do Azure Active Directory são habilitados para o locatário.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identitySecurityDefaultsEnforcementPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
