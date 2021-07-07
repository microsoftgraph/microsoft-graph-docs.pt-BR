---
title: Tipo de recurso unifiedRolePermission
description: Uma permissão de função de diretório é uma coleção de ações e condições de recursos permitidos.
localization_priority: Normal
author: sureshja
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6fc799fec39eaa209ac8e74b02743cf84e76a51a
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316474"
---
# <a name="unifiedrolepermission-resource-type"></a>Tipo de recurso unifiedRolePermission

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção de ações de recursos permitidas e as condições que devem ser atendidas para que a ação seja efetiva. Ações de recurso são tarefas que podem ser executadas em um recurso. Por exemplo, o recurso de aplicativo oferece suporte para criar, atualizar, excluir e redefinir ações de recurso de senha.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|allowedResourceActions|String collection| Conjunto de tarefas que podem ser executadas em um recurso. |
|condition|String| Restrições opcionais que devem ser atendidas para que a permissão seja efetiva. |

### <a name="allowedresourceactions-property"></a>Propriedade allowedResourceActions

Veja a seguir o esquema para ações de recurso: 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
Por exemplo: `microsoft.directory/applications/credentials/update`.  

- Namespace - Os serviços que expõem a tarefa. Por exemplo, todas as tarefas Azure Active Directory usar o namespace microsoft.directory.  
- Entidade - Os recursos lógicos ou componentes expostos pelo serviço no Microsoft Graph. Por exemplo, aplicativos, entidades de serviço ou grupos.
- PropertySet - As propriedades ou aspectos específicos da entidade para a qual o acesso está sendo concedido. Por exemplo, concede a capacidade de ler a URL de resposta, a URL de logout e a propriedade de fluxo implícito no objeto `microsoft.directory/applications/authentication/read` **application** no Azure AD. Veja a seguir os nomes reservados para conjuntos de propriedades comuns:  
  - allProperties - Designa todas as propriedades da entidade, incluindo propriedades privilegiadas. Exemplos incluem `microsoft.directory/applications/allProperties/read` `microsoft.directory/applications/allProperties/update` e .
  - basic - designa propriedades comuns de leitura, mas exclui as privilegiadas. Por exemplo, `microsoft.directory/applications/basic/update` inclui a capacidade de atualizar propriedades padrão, como o nome de exibição.
  - standard - designa propriedades de atualização comuns, mas exclui as privilegiadas. Por exemplo, `microsoft.directory/applications/standard/read`.
- Ações - As operações que estão sendo concedidas. Na maioria das circunstâncias, as permissões devem ser expressas em termos de CRUD ou allTasks. As ações incluem:
  - Criar - A capacidade de criar uma nova instância da entidade.
  - Leitura - A capacidade de ler um determinado conjunto de propriedades (incluindo allProperties).
  - Atualização - A capacidade de atualizar um determinado conjunto de propriedades (incluindo allProperties).
  - Excluir - A capacidade de excluir uma determinada entidade.
  - AllTasks - Representa todas as operações CRUD (criar, ler, atualizar e excluir). 

### <a name="condition-property"></a>propriedade condition
As condições definem restrições que devem ser atendidas. Por exemplo, um requisito de que a entidade seja um "proprietário" do destino. Veja a seguir as condições com suporte:

- Self: "$ResourceIsSelf"
- Proprietário: "$SubjectIsOwner"

A seguir, um exemplo de permissão de função com uma condição.

```json
"rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/basic/update",
                "microsoft.directory/applications/credentials/update"
            ],
            "condition":  "$SubjectIsOwner"
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

- [Permissões de função de administrador no Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) - Para obter informações sobre permissões para funções de diretório integrados.
- [Subtipos de](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) registro de aplicativo e permissões em Azure Active Directory - Para obter informações sobre permissões disponíveis para funções de diretório personalizadas. 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
