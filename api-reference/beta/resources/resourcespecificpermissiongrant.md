---
title: tipo de recurso resourceSpecificPermissionGrant
description: Especifica a permissão que um aplicativo específico do Azure AD tem.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7119d25f25b0e4f382a077ca6a1264dc22e11d5b
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51765899"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a>tipo de recurso resourceSpecificPermissionGrant

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um resourceSpecificPermissionGrant declara a permissão concedida a um aplicativo específico do AzureAD para uma instância de um recurso no Microsoft Graph.

## <a name="methods"></a>Métodos

|  Método                                                                   |  Tipo de retorno                                                                     | Descrição                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[Listar concessões de permissão de um chat](../api/chat-list-permissiongrants.md)   | [coleção resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Listar permissões concedidas em um chat específico.  |
|[Listar concessões de permissão de um grupo](../api/group-list-permissiongrants.md) | [coleção resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Listar permissões concedidas em um grupo específico. |

## <a name="properties"></a>Propriedades

| Propriedade        | Tipo          | Descrição                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| id              | string        | O identificador exclusivo da concessão de permissão específica do recurso. Somente leitura.           |
| deletedDateTime | dateTimeOffset| Não usado.                                                                             |
| clientId        | string        | ID do aplicativo do Azure AD que recebeu acesso. Somente leitura.                            |
| clientAppId     | string        | ID da entidade de serviço do aplicativo do Azure AD que recebeu acesso. Somente leitura.   |
| resourceAppId   | string        | ID do aplicativo do Azure AD que está hospedando o recurso. Somente leitura.                        |
| permissionType  | string        | O tipo de permissão. Os valores possíveis são: `Application` e `Delegated`. Somente leitura. |
| permission      | string        | O nome da permissão. Somente leitura.                                                |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant"
}-->

```json
{
  "id": "string (identifier)",
  "deletedDateTime": "dateTimeOffset",
  "clientId": "string",
  "clientAppId": "string",
  "resourceAppId": "string",
  "permissionType": "string",
  "permission": "string"
}
```


