---
title: tipo de recurso identitySecurityDefaultsEnforcementPolicy
description: Representa a política de padrões de segurança do Azure Active Directory. Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4771af4502df2154435ae6b403fa12e3e265217a
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218461"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a>tipo de recurso identitySecurityDefaultsEnforcementPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a política de [padrões de segurança](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) do Azure Active Directory. Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.

Herda de [policyBase](../resources/policybase.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | Ler as propriedades de um objeto **identitySecurityDefaultsEnforcementPolicy** . |
| [Update](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | Atualize um objeto **identitySecurityDefaultsEnforcementPolicy** . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String|Descrição da política. Somente leitura.|
|displayName|Cadeia de caracteres|Nome para exibição dessa política. Somente leitura.|
|id|String|Identificador para esta política. Somente leitura.|
|isEnabled|Boolean|Se definido como true, os padrões de segurança do Active Directory do Azure são habilitados para o locatário.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
  "baseType": "",
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
