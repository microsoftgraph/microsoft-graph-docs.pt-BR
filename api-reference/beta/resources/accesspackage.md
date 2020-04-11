---
title: tipo de recurso accessPackage
description: Um pacote do Access define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d49ddfcc0db9b55701f0b84a223efcec85aa8dfe
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228062"
---
# <a name="accesspackage-resource-type"></a>tipo de recurso accessPackage

Namespace: microsoft.graph



No [Azure ad pretitulation Management](entitlementmanagement-root.md), um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.  
Cada pacote de acesso é referenciado por um único catálogo de pacotes do Access e tem links para os recursos desse catálogo por meio de escopos de função específicos do recurso que definem o acesso que o pacote fornece.  Um pacote do Access também é vinculado às diretivas de atribuição de pacote do Access, cada um deles define quem pode solicitar ou receber uma atribuição de pacote do Access.

Para atribuir um usuário a um pacote do Access, [crie um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) que faça referência ao pacote do Access e à política de atribuição de pacotes do Access.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackages](../api/accesspackage-list.md) | coleção [accessPackage](accesspackage.md) | Recupere uma lista de objetos **accesspackage** . |
| [Criar accessPackage](../api/accesspackage-post.md) | [accessPackage](accesspackage.md) | Criar um novo objeto **accesspackage** . |
| [Obter accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | Ler propriedades e relações de um objeto **accesspackage** . |
| [Excluir accessPackage](../api/accesspackage-delete.md) |Nenhum | Excluir um **accesspackage**. |
| [Listar accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | coleção [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Recupere uma lista de objetos **accessPackageResourceRoleScope** para este pacote de acesso. |
| [Criar accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) |Nenhum | Crie um novo objeto **accessPackageResourceRoleScope** para este pacote de acesso. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|catalogID|String|ID do catálogo de pacotes do Access que faz referência a esse pacote de acesso. Somente leitura.|
|createdBy|String|O UPN do usuário ou a identidade do assunto que criou este recurso. Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|description|String|A descrição do pacote do Access.|
|displayName|Cadeia de caracteres|O nome de exibição do pacote do Access.|
|id|String| Somente leitura.|
|isHidden|Boolean|Se o pacote de acesso está oculto do solicitante.|
|isRoleScopesVisible|Boolean|Indica se os escopos de função estão visíveis.|
|modifiedBy|String|O UPN do usuário que modificou este recurso pela última vez. Somente leitura.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura. |

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageAssignmentPolicies|coleção [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Somente leitura. Anulável.|
|accessPackageCatalog|[accessPackageCatalog](accesspackagecatalog.md)| Somente leitura. Anulável.|
|accessPackageResourceRoleScopes|coleção [accessPackageResourceRoleScope](accesspackageresourcerolescope.md)| Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackage",
  "baseType": "",
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
