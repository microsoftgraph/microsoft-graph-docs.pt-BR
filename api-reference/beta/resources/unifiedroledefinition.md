---
title: Tipo de recurso unifiedRoleDefinition
description: Uma definição de função unificada é uma coleção de permissões
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 93bc01ac19e0f976463821342524b060141e6182
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247228"
---
# <a name="unifiedroledefinition-resource-type"></a>Tipo de recurso unifiedRoleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção de permissões que listam as operações, como leitura, gravação e exclusão, que podem ser executadas por um provedor RBAC, como parte do gerenciamento de função [RBAC Microsoft 365](rolemanagement.md) RBAC.

No momento, há suporte para os seguintes provedores RBAC:
- PC na nuvem. 
- gerenciamento de dispositivo (Intune)
- directory (Azure AD) 
- gerenciamento de direitos (Azure AD)


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar unifiedRoleDefinition](../api/rbacapplication-list-roledefinitions.md) | [Coleção unifiedRoleDefinition](unifiedroledefinition.md) | Leia uma lista de objetos unifiedRoleDefinition e suas propriedades. |
| [Obter unifiedRoleDefinition](../api/unifiedroledefinition-get.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Leia as propriedades de um objeto unifiedRoleDefinition. |
| [Criar roleDefinitions](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Crie um objeto unifiedRoleDefinition. |
| [Atualizar unifiedRoleDefinition](../api/unifiedroledefinition-update.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Atualize um objeto unifiedRoleDefinition. |
| [Excluir unifiedRoleDefinition](../api/unifiedroledefinition-delete.md) | Nenhum | Exclua um objeto unifiedRoleDefinition. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|Cadeia de caracteres| A descrição para unifiedRoleDefinition. Somente leitura quando **isBuiltIn** for true. |
|displayName|Cadeia de caracteres| O nome de exibição para unifiedRoleDefinition. Somente leitura quando **isBuiltIn** for true. Obrigatório.  Dá `$filter` suporte (`eq` e somente `startsWith` operadores).|
|id|Cadeia de caracteres| O identificador exclusivo para unifiedRoleDefinition. Chave, não anulável, somente leitura.  Dá suporte `$filter` (`eq` somente operador). |
|isBuiltIn|Booliano| Sinalizador que indica se unifiedRoleDefinition faz parte do conjunto padrão incluído no produto ou personalizado. Somente leitura.  Dá suporte `$filter` (`eq` somente operador).|
|isEnabled|Booliano| Sinalizador que indica se a função está habilitada para atribuição. Se for false, a função não estará disponível para atribuição. Somente leitura quando **isBuiltIn** for true. |
|resourceScopes|Coleção de cadeias de caracteres| A lista de permissões de escopos concedidas pela definição de função se aplica. Atualmente, há suporte `/` apenas. Somente leitura quando isBuiltIn for true. **NÃO USE. Isso será preterido em breve. Anexar escopo à atribuição de função** | 
|rolePermissions|[Coleção unifiedRolePermission](unifiedrolepermission.md)| Lista de permissões incluídas na função. Somente leitura quando **isBuiltIn** for true. Obrigatório. |
|Templateid|Cadeia de caracteres| Identificador de modelo personalizado que pode ser definido quando isBuiltIn é false. Esse identificador normalmente é usado se for necessário que um identificador seja o mesmo em diretórios diferentes. Somente leitura quando **isBuiltIn** for true. |
|versão|String| Indica a versão do unifiedRoleDefinition. Somente leitura quando **isBuiltIn** for true.|

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|inheritsPermissionsFrom| [Coleção unifiedRoleDefinition](unifiedroledefinition.md)| Coleção somente leitura de definições de função da qual a definição de função fornecida herda. Somente Azure AD funções internas dão suporte a esse atributo. |

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


