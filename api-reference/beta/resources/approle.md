---
title: tipo de recurso appRole
description: Representa uma função de aplicativo que podem ser solicitados por um aplicativo cliente chamar outro aplicativo ou que podem ser usadas para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificado. A propriedade **appRoles** da entidade servicePrincipal e da entidade do aplicativo é uma coleção de **appRole**.
localization_priority: Normal
ms.openlocfilehash: 6f587c15073cf2ad5f6b9973de8f7ef66c294294
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571251"
---
# <a name="approle-resource-type"></a>tipo de recurso appRole

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma função de aplicativo que podem ser solicitados por um aplicativo cliente chamar outro aplicativo ou que podem ser usadas para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificado. A propriedade **appRoles** da entidade [servicePrincipal](serviceprincipal.md) e da entidade do [aplicativo](application.md) é uma coleção de **appRole**.

> Importante: Essa funcionalidade está desabilitada na versão atual.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRole"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowedMemberTypes|String collection|Especifica se esta definição de aplicativo de função pode ser atribuída aos usuários e grupos pela configuração para "User", ou para outros aplicativos (que estão acessando este aplicativo em cenários de serviço daemon) por configuração para "Aplicativo", ou ambos.|
|description|String|Permissão ajudam o texto que aparece na atribuição app admin e experiências de consentimento.|
|displayName|String|Nome para exibição da permissão que aparece nas experiências de atribuição de consentimento e app admin.|
|id|Guid|Identificador exclusivo de função dentro da coleção **appRoles** .|
|isEnabled|Boolean|Ao criar ou atualizar uma definição de função, isso deve ser definido como **true** (o que é o padrão). Para excluir uma função, isso deve primeiro ser definido como **false**.  Nesse momento, em uma chamada subsequente, essa função pode ser removida.|
|valor|String|Especifica o valor da declaração funções que o aplicativo deve esperar em tokens de acesso e autenticação.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
