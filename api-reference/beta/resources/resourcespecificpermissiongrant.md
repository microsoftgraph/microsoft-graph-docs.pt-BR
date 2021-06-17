---
title: tipo de recurso resourceSpecificPermissionGrant
description: Especifica a permissão que um aplicativo específico do Azure AD tem.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 56d7ea203f4ed72f45a3650197c1484f817567e6
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992307"
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
|[Listar concessões de permissão de uma equipe](../api/team-list-permissiongrants.md)   | [coleção resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Listar permissões concedidas em uma equipe específica.  |

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


