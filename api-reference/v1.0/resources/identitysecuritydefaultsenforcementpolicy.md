---
title: Tipo de recurso identitySecurityDefaultsEnforcementPolicy
description: Representa a Azure Active Directory de padrões de segurança. Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.
localization_priority: Normal
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d2e3c4af8bbb7dbac35f2a28a4704010b6c6d50542d2c5de9bd1cad3cb443a90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54238087"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a>Tipo de recurso identitySecurityDefaultsEnforcementPolicy

Namespace: microsoft.graph

Representa a Azure Active Directory [de padrões de](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) segurança. Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.

Herda de [policyBase](../resources/policybase.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | Leia as propriedades de **um objeto identitySecurityDefaultsEnforcementPolicy.** |
| [Atualizar](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | Atualize **um objeto identitySecurityDefaultsEnforcementPolicy.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|Cadeia de caracteres|Descrição dessa política. Somente leitura.|
|displayName|String|Nome de exibição para esta política. Somente leitura.|
|id|Cadeia de caracteres|Identificador dessa política. Somente leitura.|
|isEnabled|Booliano|Se definido como `true` , Azure Active Directory de segurança está habilitado para o locatário.|

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
