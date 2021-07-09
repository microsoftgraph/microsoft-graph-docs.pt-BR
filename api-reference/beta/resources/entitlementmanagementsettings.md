---
title: Tipo de recurso entitlementManagementSettings
description: Representa as configurações de todo o locatário para o gerenciamento de direitos do Azure AD.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d34a04d0f8eb3bdff16befd43870b75d473a8d0c
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350975"
---
# <a name="entitlementmanagementsettings-resource-type"></a>Tipo de recurso entitlementManagementSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa configurações que controlam o comportamento do gerenciamento de direitos do [Azure AD.](entitlementmanagement-root.md)  Esse recurso não inclui a configuração de criadores de catálogos; para exibir ou alterar a associação de função de criadores de catálogo, use a [API](unifiedroleassignment.md) de atribuições de função com o provedor RBAC de gerenciamento de direitos.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Leia as propriedades de **um objeto entitlementManagementSettings.** |
| [Atualizar](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Atualize as propriedades de **um objeto entitlementManagementSettings.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|externalUserLifecycleAction|Cadeia de caracteres|Um dos `None` , `BlockSignIn` ou `BlockSignInAndDelete` . |
|daysUntilExternalUserDeletedAfterBlocked|Int64|Se **externalUserLifecycleAction** for , o número de dias após um usuário externo ser bloqueado de entrar antes de `BlockSignInAndDelete` sua conta ser excluída.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "keyProperty": ""
}-->

```json
{
  "externalUserLifecycleAction": "String",
  "daysUntilExternalUserDeletedAfterBlocked": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "entitlementManagementSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


