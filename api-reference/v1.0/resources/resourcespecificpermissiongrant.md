---
title: tipo de recurso resourceSpecificPermissionGrant
description: Especifica a permissão que um aplicativo específico do Azure AD tem.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 221576c08af5e97979d2a42e8dc0cce483e3bf35
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264154"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a>tipo de recurso resourceSpecificPermissionGrant

Namespace: microsoft.graph

Declara a permissão concedida a um aplicativo específico do Azure AD para uma instância de um recurso no Microsoft Graph.

Para obter mais informações sobre a concessão de consentimento de aplicativos para acessar uma instância específica de um recurso, consulte [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

## <a name="methods"></a>Métodos

|  Método                                                                   |  Tipo de retorno                                                                     | Descrição                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[Listar concessões de permissão de um grupo](../api/group-list-permissiongrants.md) | Coleção [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Listar permissões específicas de recursos que foram concedidas em um grupo [específico.](group.md) |

## <a name="properties"></a>Propriedades

| Propriedade        | Tipo          | Descrição                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| id              | cadeia de caracteres        | O identificador exclusivo da concessão de permissão específica do recurso. Somente leitura.           |
| deletedDateTime | dateTimeOffset| Não usado.                                                                             |
| clientId        | cadeia de caracteres        | ID do aplicativo do Azure AD que recebeu acesso. Somente leitura.                            |
| clientAppId     | cadeia de caracteres        | ID da entidade de serviço do aplicativo do Azure AD que recebeu acesso. Somente leitura.   |
| resourceAppId   | cadeia de caracteres        | ID do aplicativo do Azure AD que está hospedando o recurso. Somente leitura.                        |
| permissionType  | cadeia de caracteres        | O tipo de permissão. Os valores possíveis são: `Application` e `Delegated`. Somente leitura. |
| permission      | cadeia de caracteres        | O nome da permissão específica do recurso. Somente leitura.                                                |

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
