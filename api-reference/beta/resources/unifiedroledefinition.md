---
title: Tipo de recurso unifiedRoleDefinition
description: Uma definição de função unificada é uma coleção de permissões
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 804315ae2ae4b803088a419913ca91c11a8e51c4
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316491"
---
# <a name="unifiedroledefinition-resource-type"></a>Tipo de recurso unifiedRoleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção de permissões que listam as operações, como leitura, gravação e exclusão, que podem ser executadas [](rolemanagement.md)por um provedor RBAC, como parte do gerenciamento de função RBAC Microsoft 365 RBAC.

No momento, há suporte para os seguintes provedores RBAC:
- cloud PC 
- gerenciamento de dispositivos (Intune)
- directory (Azure AD) 
- gerenciamento de direitos (Azure AD)

> [!NOTE]
> No momento, os provedores de RBAC de gerenciamento de direitos e pc na nuvem suportam apenas a [lista](../api/rbacapplication-list-roledefinitions.md) e [obter](../api/unifiedroledefinition-get.md) operações.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar unifiedRoleDefinition](../api/rbacapplication-list-roledefinitions.md) | [Coleção unifiedRoleDefinition](unifiedroledefinition.md) | Leia uma lista de objetos unifiedRoleDefinition e suas propriedades. |
| [Obter unifiedRoleDefinition](../api/unifiedroledefinition-get.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Leia as propriedades de um objeto unifiedRoleDefinition. |
| [Criar unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Crie um objeto unifiedRoleDefinition. |
| [Atualizar unifiedRoleDefinition](../api/unifiedroledefinition-update.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Atualize um objeto unifiedRoleDefinition. |
| [Excluir unifiedRoleDefinition](../api/unifiedroledefinition-delete.md) | Nenhum | Exclua um objeto unifiedRoleDefinition. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String| A descrição do unifiedRoleDefinition. Somente leitura quando **isBuiltIn** for true. |
|displayName|String| O nome de exibição do unifiedRoleDefinition. Somente leitura quando **isBuiltIn** for true. Obrigatório.  Oferece `$filter` suporte ( e somente `eq` `startsWith` operadores).|
|id|String| O identificador exclusivo do unifiedRoleDefinition. Chave, não anulada, somente leitura.  Suporta `$filter` ( `eq` somente operador). |
|isBuiltIn|Booliano| Sinalizador indicando se unifiedRoleDefinition faz parte do conjunto padrão incluído no produto ou personalizado. Somente leitura.  Suporta `$filter` ( `eq` somente operador).|
|isEnabled|Booliano| Sinalizador indicando se a função está habilitada para atribuição. Se for false, a função não estará disponível para atribuição. Somente leitura quando **isBuiltIn** for true. |
|resourceScopes|Coleção de cadeias de caracteres| Lista de permissões de escopo concedidas pela definição de função a que se aplicam. Atualmente, `/` só há suporte. Somente leitura quando isBuiltIn for true. **NÃO USE. Isso será preterido em breve. Anexar escopo à atribuição de função** | 
|rolePermissions|[Coleção unifiedRolePermission](unifiedrolepermission.md)| Lista de permissões incluídas na função. Somente leitura quando **isBuiltIn** for true. Obrigatório. |
|templateId|String| Identificador de modelo personalizado que pode ser definido quando isBuiltIn é false. Esse identificador normalmente é usado se um identificador precisa ser o mesmo em diretórios diferentes. Somente leitura quando **isBuiltIn** for true. |
|versão|String| Indica a versão do unifiedRoleDefinition. Somente leitura quando **isBuiltIn** for true.|

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|inheritsPermissionsFrom| [Coleção unifiedRoleDefinition](unifiedroledefinition.md)| Coleção somente leitura de definições de função que a definição de função determinada herda. Somente funções do Azure AD integrados suportam esse atributo. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isBuiltIn": true,
  "isEnabled": true,
  "resourceScopes": ["String"],
  "rolePermissions": [{"@odata.type": "microsoft.graph.unifiedRolePermission"}],
  "templateId": "String",
  "inheritsPermissionsFrom": [{"@odata.type": "microsoft.graph.unifiedRoleDefinition"}],
  "version": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


