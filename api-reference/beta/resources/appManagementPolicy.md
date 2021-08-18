---
title: Tipo de recurso appManagementPolicy
description: Uma política de método de auth de aplicativos para impor restrições de gerenciamento de aplicativos a entidades de serviço ou aplicativos específicos.
author: madansr7
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c34d9c285b4add5976603f8b9dafa4c67dd94b7d
ms.sourcegitcommit: b7e01a1331abe5f5c9aa2828d93dad08229573f1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58336867"
---
# <a name="appmanagementpolicy-resource-type"></a>Tipo de recurso appManagementPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Restrições às operações de gerenciamento de aplicativos para aplicativos específicos e entidades de serviço. Se esse recurso não estiver configurado para um aplicativo ou entidade de serviço, as restrições padrão para as configurações no [objeto tenantAppManagementPolicy.](tenantappmanagementpolicy.md)

## <a name="methods"></a>Métodos

| Método                                                         | Tipo de retorno                                                                | Descrição                                                                                                            |
| :------------------------------------------------------------- | :------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------- |
| [List](../api/appManagementPolicy-list.md)      | [appManagementPolicy](../resources/appManagementPolicy.md) | Retorna uma lista de políticas de gerenciamento de aplicativos criadas para aplicativos e entidades de serviço juntamente com suas propriedades. |
| [Create](../api/appManagementPolicy-post.md)    | [appManagementPolicy](../resources/appManagementPolicy.md) | Cria uma política de gerenciamento de aplicativos que pode ser atribuída a um objeto de entidade de serviço ou aplicativo.                   |
| [Get](../api/appManagementPolicy-get.md)       | [appManagementPolicy](../resources/appManagementPolicy.md) | Obtém um único objeto de política de gerenciamento de aplicativo.                                                                            |
| [Atualizar](../api/appManagementPolicy-update.md) | Nenhum(a)                                                                       | Atualiza uma política de gerenciamento de aplicativos.                                                                                      |
| [Delete](../api/appManagementPolicy-delete.md) | Nenhum                                                                       | Exclui uma política de gerenciamento de aplicativos da coleção de políticas em appManagementPolicies.                             |
| [Lista appliesTo](../api/appManagementPolicy-list-appliesTo.md)| [appManagementPolicy](../resources/appManagementPolicy.md)|Retorna uma lista de aplicativos e entidades de serviço às quais a política é aplicada. |
| [Atribuir appliesTo](../api/appManagementPolicy-post-appliesTo.md)| Nenhum |Retorna uma lista de aplicativos e entidades de serviço às quais a política é aplicada. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo                                                        | Descrição                                                            |
| :----------- | :---------------------------------------------------------- | :--------------------------------------------------------------------- |
| id           | Cadeia de caracteres                                                      | O identificador de política.                                                 |
| displayName  | Cadeia de caracteres                                                      | O nome de exibição da política. Herdado de [policyBase](policybase.md).                                        |
| description  | Cadeia de caracteres                                                      | A descrição da política. Herdado de [policyBase](policybase.md).                                         |
| isEnabled    | Booliano                                                     | Indica se a política está habilitada.                                      |
| restrictions | [appManagementConfiguration](appManagementConfiguration.md) | Restrições que se aplicam a um objeto de entidade de serviço ou aplicativo. |

## <a name="relationships"></a>Relações

| Relação | Tipo                                  | Descrição                                                                         |
| :----------- | :------------------------------------ | :---------------------------------------------------------------------------------- |
| appliesTo    | [directoryObject](directoryobject.md) | Coleção de entidades de serviço e aplicativos às quais uma política é aplicada. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appManagementPolicy",
  "baseType": "microsoft.graph.policyBase",
  "openType": false
}
-->

```json
[
  {
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/appManagementPolicies",
    "id": "string (identifier)",
    "description": "string",
    "displayName": "string",
    "isEnabled": true,
    "restrictions": {
      "@odata.type": "microsoft.graph.appManagementConfiguration"
    }
  }
]
```
