---
title: Tipo de recurso appManagementPolicy
description: Uma política de método de auth de aplicativos para impor restrições de gerenciamento de aplicativos a entidades de serviço ou aplicativos específicos.
author: madansr7
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c3a705a567e4692d07220398317cc36c2bab71a6
ms.sourcegitcommit: b711aed8acc18512cf6591f4108ed5ddf05b649d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2021
ms.locfileid: "53660355"
---
# <a name="appmanagementpolicy-resource-type"></a>Tipo de recurso appManagementPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Impor restrições às operações de gerenciamento de aplicativos para aplicativos e entidades de serviço específicas. Se esse recurso não estiver configurado para um aplicativo ou entidade de serviço, as restrições padrão para as configurações no [objeto tenantAppManagementPolicy.](tenantappmanagementpolicy.md)

## <a name="methods"></a>Métodos

| Método                                                         | Tipo de retorno                                                                | Descrição                                                                                                            |
| :------------------------------------------------------------- | :------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------- |
| [List](../api/appManagementPolicy-list.md)      | [appManagementPolicy](../resources/appManagementPolicy.md) | Retorna uma lista de políticas de gerenciamento de aplicativos criadas para aplicativos e entidades de serviço juntamente com suas propriedades. |
| [Criar](../api/appManagementPolicy-post.md)    | [appManagementPolicy](../resources/appManagementPolicy.md) | Cria uma política de gerenciamento de aplicativos que pode ser atribuída a um objeto de entidade de serviço ou aplicativo.                   |
| [Obter](../api/appManagementPolicy-get.md)       | [appManagementPolicy](../resources/appManagementPolicy.md) | Obtém um único objeto de política de gerenciamento de aplicativo.                                                                            |
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
