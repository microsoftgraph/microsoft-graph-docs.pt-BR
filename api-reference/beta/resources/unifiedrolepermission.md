---
title: Tipo de recurso unifiedRolePermission
description: Uma permissão de função de diretório é um conjunto de ações e condições de recursos permitidos.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f19ecbb4672ec877371621d7c96284f683f600db
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934871"
---
# <a name="unifiedrolepermission-resource-type"></a>Tipo de recurso unifiedRolePermission

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção de ações de recurso permitidas e as condições que devem ser atendidas para que a ação seja efetiva. Ações de recurso são tarefas que podem ser baseadas em um recurso. Por exemplo, o recurso de aplicativo oferece suporte para criar, atualizar, excluir e redefinir ações de recurso de senha.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|allowedResourceActions|String collection| Conjunto de tarefas que podem ser executadas em um recurso. |
|condição|Cadeia de caracteres| Restrições opcionais que devem ser atendidas para que a permissão seja efetiva. |

### <a name="allowedresourceactions-property"></a>Propriedade allowedResourceActions

Este é o esquema para ações de recurso: 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
Por exemplo: `microsoft.directory/applications/credentials/update`.  

- Namespace - Os serviços que expõem a tarefa. Por exemplo, todas as tarefas no Azure Active Directory usam o namespace microsoft.directory.  
- Entidade - Os recursos lógicos ou componentes expostos pelo serviço no Microsoft Graph. Por exemplo, aplicativos, entidades de serviço ou grupos.
- PropertySet - As propriedades ou aspectos específicos da entidade para a qual o acesso está sendo concedido. Por exemplo, concede a capacidade de ler a URL de resposta, a URL de logout e a propriedade de fluxo implícita no objeto do aplicativo no `microsoft.directory/applications/authentication/read` Azure  AD. A seguir estão os nomes reservados para conjuntos de propriedades comuns:  
  - allProperties - Designa todas as propriedades da entidade, incluindo propriedades privilegiadas. Exemplos incluem `microsoft.directory/applications/allProperties/read` e `microsoft.directory/applications/allProperties/update` .
  - básico - Designa propriedades de leitura comuns, mas exclui as privilegiadas. Por exemplo, `microsoft.directory/applications/basic/update` inclui a capacidade de atualizar propriedades padrão, como nome para exibição.
  - padrão - Designa propriedades de atualização comuns, mas exclui as privilegiadas. Por exemplo, `microsoft.directory/applications/standard/read`.
- Ações - As operações que estão sendo concedidas. Na maioria das circunstâncias, as permissões devem ser expressas em termos crud ou allTasks. As ações incluem:
  - Criar - a capacidade de criar uma nova instância da entidade.
  - Read - A capacidade de ler um determinado conjunto de propriedades (incluindo allProperties).
  - Atualização - a capacidade de atualizar um determinado conjunto de propriedades (incluindo allProperties).
  - Excluir - A capacidade de excluir uma determinada entidade.
  - AllTasks – Representa todas as operações CRUD (criar, ler, atualizar e excluir). 

### <a name="condition-property"></a>propriedade condition
As condições definem restrições que devem ser atendidas. Por exemplo, um requisito de que o diretor seja um "proprietário" do destino. A seguir estão as condições com suporte:

- Self: "$ResourceIsSelf"
- Proprietário: "$SubjectIsOwner"

A seguir está um exemplo de uma permissão de função com uma condição.

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
- [Subtipos e](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) permissões de registro de aplicativo no Azure Active Directory - Para obter informações sobre permissões que estão disponíveis para funções de diretório personalizadas. 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
