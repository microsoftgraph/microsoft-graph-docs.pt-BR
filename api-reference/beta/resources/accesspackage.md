---
title: Tipo de recurso accessPackage
description: Um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2d288465b04986b98de7b67fa049657b8bcf0a58
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298528"
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
| [Atualizar accessPackage](../api/accesspackage-update.md)|Nenhum(a) | Atualize as propriedades de um **objeto accesspackage.** |
| [Excluir accessPackage](../api/accesspackage-delete.md) |Nenhum(a) | Excluir um **accesspackage**. |
| [Listar accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [Coleção accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Recupere uma lista de **objetos accessPackageResourceRoleScope** para este pacote de acesso. |
| [Criar accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) |Nenhum(a) | Crie um novo **objeto accessPackageResourceRoleScope** para este pacote de acesso. |
|[filterByCurrentUser](../api/accesspackage-filterbycurrentuser.md)|[Coleção accessPackage](../resources/accesspackage.md)|Recupere a lista de **objetos accessPackage** filtrados no usuário de entrada.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|catalogId|Cadeia de caracteres|ID do catálogo de pacotes de acesso referenciando este pacote de acesso. Somente leitura.|
|createdBy|Cadeia de caracteres|UPN do usuário ou identidade do assunto que criou esse recurso. Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|description|Cadeia de caracteres|A descrição do pacote de acesso.|
|displayName|Cadeia de caracteres|O nome de exibição do pacote de acesso.|
|id|String| Somente leitura.|
|isHidden|Booliano|Se o pacote de acesso está oculto do solicitante.|
|isRoleScopesVisible|Booliano|Indica se os escopos de função estão visíveis.|
|modifiedBy|Cadeia de caracteres|O UPN do usuário que modificou esse recurso pela última vez. Somente leitura.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageAssignmentPolicies|[coleção accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Somente leitura. Anulável.|
|accessPackageCatalog|[accessPackageCatalog](accesspackagecatalog.md)| Somente leitura. Anulável.|
|accessPackageResourceRoleScopes|[Coleção accessPackageResourceRoleScope](accesspackageresourcerolescope.md)| Anulável.|

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


