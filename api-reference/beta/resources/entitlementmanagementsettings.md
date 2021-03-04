---
title: Tipo de recurso entitlementManagementSettings
description: Representa as configurações de todo o locatário para o gerenciamento de direitos do Azure AD.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b4b6ee584e671e070955eb7c065c59cb8481c375
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440350"
---
# <a name="entitlementmanagementsettings-resource-type"></a>Tipo de recurso entitlementManagementSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa configurações que controlam o comportamento do gerenciamento de direitos do [Azure AD.](entitlementmanagement-root.md)

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Leia as propriedades de **um objeto entitlementManagementSettings.** |
| [Atualização](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Atualize as propriedades de **um objeto entitlementManagementSettings.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|externalUserLifecycleAction|String|Um dos `None` , `BlockSignIn` ou `BlockSignInAndDelete` . |
|daysUntilExternalUserDeletedAfterBlocked|Int64|Se for , o número de dias após um usuário externo ser bloqueado de `externalUserLifecycleAction` entrar antes que sua conta seja `BlockSignInAndDelete` excluída.|

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


