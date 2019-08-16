---
title: tipo de recurso unifiedRolePermission
description: Uma permissão de função de diretório é uma coleção de ações e condições de recursos permitidas.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d15e2709c429be3c6400b59db5174093892d3009
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437857"
---
# <a name="unifiedrolepermission-resource-type"></a>tipo de recurso unifiedRolePermission

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção de ações de recurso permitidas e as condições que devem ser atendidas para que a ação seja eficaz. Ações de recurso são tarefas que podem ser perfomed em um recurso. Por exemplo, o recurso de aplicativo suporta criar, atualizar, excluir e redefinir ações de recurso de senha.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|allowedResourceActions|String collection| Conjunto de tarefas que podem ser perfomed em um recurso. |
|pré-requisito|String| Restrições opcionais que devem ser atendidas para que a permissão seja eficaz. |

### <a name="allowedresourceactions-property"></a>Propriedade allowedResourceActions

Veja a seguir o esquema para ações de recurso: 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
Por exemplo: `microsoft.directory/applications/credentials/update`.  

- Namespace-os serviços que expõem a tarefa. Por exemplo, todas as tarefas no Azure Active Directory usam o namespace Microsoft. Directory.  
- Entidade – os recursos ou componentes lógicos expostos pelo serviço no Microsoft Graph. Por exemplo, aplicativos, entidades de serviço ou grupos.
- PropertySet-as propriedades específicas ou aspectos da entidade para a qual o acesso está sendo concedido. Por exemplo, `microsoft.directory/applications/authentication/read` concede a capacidade de ler a URL de resposta, a URL de logout e a propriedade de fluxo implícito no objeto **Application** no Azure AD. Estes são os nomes reservados para conjuntos de propriedades comuns:  
  - Propriedades: designa todas as propriedades da entidade, incluindo propriedades privilegiadas. Os exemplos `microsoft.directory/applications/allProperties/read` incluem `microsoft.directory/applications/allProperties/update`e.
  - Basic-designa Propriedades de leitura comuns, mas exclui privilégios privilegiados. Por exemplo, `microsoft.directory/applications/basic/update` inclui a capacidade de atualizar propriedades padrão, como o nome para exibição.
  - Standard-designa Propriedades comuns de atualização, mas exclui privilégios privilegiados. Por exemplo, `microsoft.directory/applications/standard/read`.
- Ações-as operações que estão sendo concedidas. Na maioria das circunstâncias, as permissões devem ser expressas em termos de CRUD ou de tarefas. As ações incluem:
  - Create-a capacidade de criar uma nova instância da entidade.
  - Read-a capacidade de ler um determinado conjunto de Propriedades (incluindo itempropertys).
  - Update-a capacidade de atualizar um determinado conjunto de Propriedades (incluindo itempropertys).
  - Delete-a capacidade de excluir uma determinada entidade.
  - Multitasks-representa todas as operações CRUD (criar, ler, atualizar e excluir). 

### <a name="condition-property"></a>Propriedade Condition
As condições definem as restrições que devem ser atendidas. Por exemplo, um requisito de que a entidade seja um "proprietário" do destino. A seguir estão as condições com suporte:

- Self: "@Subject. objectId = = @Resource. objectId"
- Proprietário: "@Subject. objectId Any_of @Resource. Owners"

Veja a seguir um exemplo de permissão de função com uma condição.

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
  "allowedResourceActions": ["String"],
  "condition": "String"
}
```
## <a name="see-also"></a>Confira também

- [Permissões de função de administrador no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles) – para obter informações sobre permissões para funções de diretório internas.
- [Subtipos de registro de aplicativo e permissões no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/roles-custom-available-permissions) – para obter informações sobre permissões que estão disponíveis para funções de diretório personalizado. 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
