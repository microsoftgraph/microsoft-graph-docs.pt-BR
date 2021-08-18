---
title: Tipo de recurso accessPackage
description: Um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 95bf04ace23b6340fcef3c0945fad1bd221e8a12
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58256153"
---
# <a name="accesspackage-resource-type"></a>Tipo de recurso accessPackage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management](entitlementmanagement-root.md), um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.  

Cada pacote de acesso é referenciado por um catálogo de pacotes de acesso único e tem links para os recursos desse catálogo por meio dos escopos de função específicos do recurso que definem o acesso que o pacote fornece.  Um pacote de acesso também se vincula às políticas de atribuição de pacote de acesso, cada uma das quais define quem pode solicitar ou ser atribuído a uma atribuição de pacote de acesso.

Para atribuir um usuário a um pacote de acesso, [crie um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) que faz referência ao pacote de acesso e à política de atribuição de pacote de acesso.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackages](../api/accesspackage-list.md) | [Coleção accessPackage](accesspackage.md) | Recupere uma lista de **objetos accesspackage.** |
| [Criar accessPackage](../api/accesspackage-post.md) | [accessPackage](accesspackage.md) | Crie um novo **objeto accesspackage.** |
| [Obter accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | Ler propriedades e relações de um **objeto accesspackage.** |
| [Atualizar accessPackage](../api/accesspackage-update.md)|Nenhum | Atualize as propriedades de um **objeto accesspackage.** |
| [Excluir accessPackage](../api/accesspackage-delete.md) |Nenhum | Excluir um **accesspackage**. |
| [Listar accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [Coleção accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Recupere uma lista de **objetos accessPackageResourceRoleScope** para este pacote de acesso. |
| [Criar accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) |Nenhum | Crie um novo **objeto accessPackageResourceRoleScope** para este pacote de acesso. |
| [Listar incompatívelAccessPackages](../api/accesspackage-list-incompatibleaccesspackages.md) | [Coleção accessPackage](accesspackage.md) | Recupere uma lista dos objetos **accesspackage** incompatíveis para este pacote de acesso. |
| [Adicionar accessPackage a incompatibleAccessPackages](../api/accesspackage-post-incompatibleaccesspackage.md) | Nenhum | Adicione um link para indicar que outro **pacote de acessos** é incompatível com um pacote de acesso especificado. |
| [Remover accessPackage de incompatívelAccessPackages](../api/accesspackage-delete-incompatibleaccesspackage.md) | Nenhum | Remover um link que indicava que um **pacote de acesso** era incompatível. |
| [Listar incompatibleGroups](../api/accesspackage-list-incompatiblegroups.md) | Coleção [group](group.md) | Recupere uma lista dos objetos **de** grupo incompatíveis para este pacote de acesso. |
| [Adicionar grupo a incompatibleGroups](../api/accesspackage-post-incompatiblegroup.md) | Nenhum | Adicione um link para indicar que a associação de um **grupo** é incompatível com um pacote de acesso especificado. |
| [Remover grupo de incompatibleGroups](../api/accesspackage-delete-incompatiblegroup.md) | Nenhum | Remover um link que indicava que uma associação **ao** grupo era incompatível.|
| [Listar accessPackagesIncompatibleWith](../api/accesspackage-list-accesspackagesincompatiblewith.md) | [Coleção accessPackage](accesspackage.md) | Recupere uma lista dos  **objetos accesspackage que** listam esse pacote de acesso como incompatível. |
|[filterByCurrentUser](../api/accesspackage-filterbycurrentuser.md)|[Coleção accessPackage](../resources/accesspackage.md)|Recupere a lista de **objetos accessPackage** filtrados no usuário de entrada.|
| [getApplicablePolicyRequirements](../api/accesspackage-getapplicablepolicyrequirements.md) | [coleção accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md) | Recupere uma lista de **objetos accessPackageAssignmentRequestRequirement** com requisitos de solicitação. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|catalogId|Cadeia de caracteres|ID do catálogo de pacotes de acesso referenciando este pacote de acesso. Somente leitura.|
|createdBy|Cadeia de caracteres|UPN do usuário ou identidade do assunto que criou esse recurso. Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|description|Cadeia de caracteres|A descrição do pacote de acesso.|
|displayName|Cadeia de caracteres|O nome de exibição do pacote de acesso.|
|id|String| Somente leitura.|
|IsHidden|Booleano|Se o pacote de acesso está oculto do solicitante.|
|isRoleScopesVisible|Boolean|Indica se os escopos de função estão visíveis.|
|modifiedBy|Cadeia de caracteres|O UPN do usuário que modificou esse recurso pela última vez. Somente leitura.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageAssignmentPolicies|[coleção accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Somente leitura. Anulável.|
|accessPackageCatalog|[accessPackageCatalog](accesspackagecatalog.md)| Somente leitura. Anulável.|
|accessPackageResourceRoleScopes|[Coleção accessPackageResourceRoleScope](accesspackageresourcerolescope.md)| Anulável.|
| incompatibleAccessPackages | [Coleção accessPackage](accesspackagecatalog.md) | Os pacotes de acesso cujos usuários atribuídos são inelegíveis para serem atribuídos a esse pacote de acesso. |
| accessPackagesIncompatibleWith | [Coleção accessPackage](accesspackagecatalog.md) | Os pacotes de acesso incompatíveis com esse pacote. Somente leitura. |
| incompatibleGroups | Coleção [group](group.md) | Os grupos cujos membros são inelegíveis para serem atribuídos a este pacote de acesso. |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackage",
  "keyProperty": "id"
}-->

```json
{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package",
    "displayName":"Access package for testing",
    "isHidden":false,
    "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
    "isRoleScopesVisible":false,
    "createdDateTime":"2019-01-27T18:19:50.74Z",
    "modifiedDateTime":"2019-01-27T18:19:50.74Z",
    "createdBy":"TestGA@example.com",
    "modifiedBy":"TestGA@example.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


