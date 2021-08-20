---
title: Tipo de recurso tenantAppManagementPolicy
description: A política padrão de locatário de método de auth de aplicativo impõe restrições de operação de gerenciamento de aplicativos.
author: madansr7
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e5177fe5bc69a3f083619823146c605152498d71
ms.sourcegitcommit: 6f04ad0e0cde696661511dcdf343942b43f73fc6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2021
ms.locfileid: "58397107"
---
# <a name="tenantappmanagementpolicy-resource-type"></a>Tipo de recurso tenantAppManagementPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Política de método de autenticação de aplicativos em todo o locatário para impor restrições de gerenciamento de aplicativos para todos os aplicativos e entidades de serviço. Essa política se aplica a todos os aplicativos e entidades de serviço, a menos que seja substituído quando um [appManagementPolicy](../resources/appmanagementpolicy.md) é aplicado ao objeto.

Herda de [policyBase](policybase.md).

## <a name="methods"></a>Métodos

| Método                                                | Tipo de retorno                                                             | Descrição                                                                         |
| :---------------------------------------------------- | :---------------------------------------------------------------------- | :---------------------------------------------------------------------------------- |
| [Get](../api/tenantAppManagementPolicy-get.md)       | [tenantAppManagementPolicy](../resources/tenantAppManagementPolicy.md) | Leia as propriedades do conjunto de políticas de gerenciamento de aplicativo padrão para aplicativos e entidades de serviço. |
| [Atualizar](../api/tenantAppManagementPolicy-update.md) | Nenhum(a)                                                                    | Atualiza a política de gerenciamento de aplicativo padrão para aplicativos e entidades de serviço.  |

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                                                                     | Descrição                                                           |
| :--------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| id                           | Cadeia de caracteres                                                                   | O identificador de política padrão.                                        |
| displayName                  | Cadeia de caracteres                                                                   | O nome de exibição da política padrão. Herdado de [policyBase](policybase.md).                                |
| description                  | Cadeia de caracteres                                                                   | A descrição da política padrão. Herdado de [policyBase](policybase.md).                                |
| isEnabled                    | Booliano                                                                  | Indica se a política está habilitada. O valor padrão é `false`.                                    |
| applicationRestrictions      | [appManagementConfiguration](../resources/appManagementConfiguration.md) | Restrições que se aplicam como padrão a todos os objetos de aplicativo no locatário.               |
| servicePrincipalRestrictions | [appManagementConfiguration](../resources/appManagementConfiguration.md) | Restrições que se aplicam como padrão a todos os objetos de entidade de serviço no locatário. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tenantAppManagementPolicy",
  "baseType": "microsoft.graph.policyBase",
  "openType": false
}
-->

```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/defaultAppManagementPolicy",
  "id": "string (identifier)",
  "description": "string",
  "displayName": "string",
  "isEnabled": false,
  "applicationRestrictions": {
    "@odata.type":"microsoft.graph.appManagementConfiguration"
  },
  "servicePrincipalRestrictions": {
    "@odata.type":"microsoft.graph.appManagementConfiguration"
  }
}
```
