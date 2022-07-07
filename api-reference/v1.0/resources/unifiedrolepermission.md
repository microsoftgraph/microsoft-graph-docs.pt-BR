---
title: Tipo de recurso unifiedRolePermission
description: Uma permissão de função de diretório é uma coleção de ações e condições de recursos permitidas.
ms.localizationpriority: medium
author: sureshja
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 66c28bff1d6204dbe1a19a75bf1b9c47de6b502e
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671399"
---
# <a name="unifiedrolepermission-resource-type"></a>Tipo de recurso unifiedRolePermission

Namespace: microsoft.graph

Representa uma coleção de ações de recurso permitidas e as condições que devem ser atendidas para que a ação seja permitida. As ações de recurso são tarefas que podem ser executadas em um recurso. Por exemplo, um recurso de aplicativo pode dar suporte a ações de criação, atualização, exclusão e redefinição de senha.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|allowedResourceActions|String collection| Conjunto de tarefas que podem ser executadas em um recurso. Obrigatório. |
|Condição|String| Restrições opcionais que devem ser atendidas para que a permissão seja efetiva. |
|excludedResourceActions|Coleção de cadeias de caracteres| Conjunto de tarefas que podem não ser executadas em um recurso. Ainda não há suporte. |

### <a name="allowedresourceactions-property"></a>Propriedade allowedResourceActions

A seguir está o esquema para ações de recurso: 

```
{Namespace}/{Entity}/{PropertySet}/{Action}  
```
Por exemplo: `microsoft.directory/applications/credentials/update`.  

- *{Namespace}* - Os serviços que expõem a tarefa. Por exemplo, todas as tarefas no Azure Active Directory usam o namespace `microsoft.directory`.  
- *{Entity}* - Os recursos lógicos ou componentes expostos pelo serviço no Microsoft Graph. Por exemplo, `applications`, `servicePrincipals`ou `groups`.
- *{PropertySet}* - Opcional. As propriedades ou aspectos específicos da entidade para a qual o acesso está sendo concedido. Por exemplo, `microsoft.directory/applications/authentication/read` concede a capacidade de ler a URL de resposta, a URL de logoff e a propriedade de fluxo  implícita no objeto de aplicativo em Azure AD. A seguir estão os nomes reservados para conjuntos de propriedades comuns:  
  - `allProperties` – Designa todas as propriedades da entidade, incluindo propriedades privilegiadas. Os exemplos incluem `microsoft.directory/applications/allProperties/read` e `microsoft.directory/applications/allProperties/update`.
  - `basic` – Designa propriedades de leitura comuns, mas exclui as privilegiadas. Por exemplo, `microsoft.directory/applications/basic/update` inclui a capacidade de atualizar propriedades padrão, como o nome de exibição.
  - `standard` – Designa propriedades de atualização comuns, mas exclui as privilegiadas. Por exemplo, `microsoft.directory/applications/standard/read`.
- *{Actions}* - As operações que estão sendo concedidas. Na maioria das circunstâncias, as permissões devem ser expressas em termos de operações CRUD ou `allTasks`. Ações incluem:
  - `create` – A capacidade de criar uma nova instância da entidade.
  - `read` - A capacidade de ler um determinado conjunto de propriedades (incluindo allProperties).
  - `update` - A capacidade de atualizar um determinado conjunto de propriedades (incluindo allProperties).
  - `delete` - A capacidade de excluir uma determinada entidade.
  - `allTasks` - Representa todas as operações CRUD (criar, ler, atualizar e excluir). 

### <a name="condition-property"></a>propriedade condition
As condições definem restrições que devem ser atendidas. Por exemplo, um requisito de que a entidade de segurança seja um proprietário do recurso de destino. A seguir estão as condições com suporte:

- `Self`: "@Subject.objectId == @Resource.objectId"
- `Owner`: "@Subject.objectId Any_of @Resource.owners"

A seguir está um exemplo de uma permissão de função com uma condição de que a entidade de segurança seja o proprietário do recurso de destino.

```json
"rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/basic/update",
                "microsoft.directory/applications/credentials/update"
            ],
            "condition":  "@Subject.objectId Any_of @Resource.owners"
        }
    ]

```

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRolePermission",
  "baseType": null
}-->

```json
{
  "@odata.type": "#microsoft.graph.unifiedRolePermission",
  "allowedResourceActions": ["String"],
  "excludedResourceActions": ["String"],
  "condition": "String"
}
```
## <a name="see-also"></a>Confira também

- [Permissões de função de administrador no Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) – para obter informações sobre permissões para funções de diretório internas.
- [Subtipos e permissões de registro de aplicativo no Azure Active Directory](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) – para obter informações sobre permissões disponíveis para funções de diretório personalizadas. 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->