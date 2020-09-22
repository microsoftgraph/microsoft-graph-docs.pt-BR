---
title: tipo de recurso entitlementManagementSettings
description: Representa as configurações de todos os locatários para o gerenciamento de qualificação do Azure AD.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 84f34740bd5e16bb001cd3618edf4c4b669155f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052879"
---
# <a name="entitlementmanagementsettings-resource-type"></a>tipo de recurso entitlementManagementSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações que controlam o comportamento do [Gerenciamento de qualificação do Azure ad](entitlementmanagement-root.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Ler as propriedades de um objeto **entitlementManagementSettings** . |
| [Atualizar](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Atualiza as propriedades de um objeto **entitlementManagementSettings** . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|externalUserLifecycleAction|Cadeia de caracteres|Um de `None` , `BlockSignIn` ou `BlockSignInAndDelete` . |
|daysUntilExternalUserDeletedAfterBlocked|Int64|Se `externalUserLifecycleAction` for `BlockSignInAndDelete` , o número de dias após o qual um usuário externo é bloqueado de entrar antes que sua conta seja excluída.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "baseType": "",
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


