---
title: tipo de recurso appRole
description: Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente que esteja chamando outro aplicativo ou que possa ser usada para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificada. A propriedade **appRoles** da entidade servicePrincipalName e da entidade Application é uma coleção de **appRole**.
localization_priority: Normal
ms.openlocfilehash: 8a367406c64cf9d0d3da49716aeaf6ca3c1fa687
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535695"
---
# <a name="approle-resource-type"></a>tipo de recurso appRole

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente que esteja chamando outro aplicativo ou que possa ser usada para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificada. A propriedade **appRoles** da entidade [servicePrincipalName](serviceprincipal.md) e da entidade [Application](application.md) é uma coleção de **appRole**.

> Importante: essa funcionalidade está desabilitada na versão atual.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approle"
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
|allowedMemberTypes|Coleção de cadeias de caracteres|Especifica se essa definição de função de aplicativo pode ser atribuída a usuários e grupos por meio da configuração de "usuário" ou a outros aplicativos (que estão acessando esse aplicativo em cenários de serviço de daemon) definindo como "aplicativo" ou ambos.|
|description|String|Texto de ajuda de permissão que aparece nas experiências de consentimento e atribuição de aplicativo de administração.|
|displayName|String|Nome para exibição da permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.|
|id|Guid|Identificador de função exclusivo dentro da coleção **appRoles** .|
|isEnabled|Boolean|Ao criar ou atualizar uma definição de função, isso deve ser definido como **true** (que é o padrão). Para excluir uma função, é necessário primeiro defini-la como **false**.  Nesse ponto, em uma chamada subsequente, essa função pode ser removida.|
|value|Cadeia de caracteres|Especifica o valor da declaração de funções que o aplicativo deve esperar nos tokens de autenticação e acesso.|

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
