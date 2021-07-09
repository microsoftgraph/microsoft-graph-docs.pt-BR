---
title: Tipo de recurso accessPackageCatalog
description: Um catálogo de pacotes de acesso é um contêiner para pacotes de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 051657b5c8c7edb51a4c2c5c3a15bf3740052b86
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351094"
---
# <a name="accesspackagecatalog-resource-type"></a>Tipo de recurso accessPackageCatalog

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)um catálogo de pacotes de acesso é um contêiner para zero ou mais pacotes de acesso. Um catálogo de pacotes de acesso também pode ter recursos vinculados usados nesses pacotes de acesso para fornecer acesso. Para exibir ou alterar a associação de funções com escopo de catálogo, use a [API](unifiedroleassignment.md) de atribuições de função com o provedor RBAC de gerenciamento de direitos.



## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageCatalogs](../api/accesspackagecatalog-list.md) | [Coleção accessPackageCatalog](accesspackagecatalog.md) | Recupere uma lista de objetos accesspackagecatalog. |
| [Criar accessPackageCatalog](../api/accesspackagecatalog-post.md) | [accessPackageCatalog](accesspackagecatalog.md) | Crie um novo objeto accessPackageCatalog. |
| [Obter accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Ler propriedades e relações de um objeto accessPackageCatalog. |
| [Atualizar accessPackageCatalog](../api/accesspackagecatalog-update.md)|Nenhuma | Atualize as propriedades de um objeto accessPackageCatalog. |
| [Excluir accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | Exclua accessPackageCatalog. |
| [Listar recursos do accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresources.md) | [Coleção accessPackageResource](accesspackageresource.md) | Recupere uma lista de objetos accessPackageResource em um catálogo. |
| [Listar funções de recurso accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [Coleção accessPackageResourceRole](accesspackageresourcerole.md) | Recupere uma lista de objetos accessPackageResourceRole para recursos em um catálogo. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|catalogStatus|Cadeia de caracteres|Tem o valor `Published` se os pacotes de acesso estão disponíveis para gerenciamento.|
|catalogType|Cadeia de caracteres|Um dos `UserManaged` ou `ServiceDefault` . |
|createdBy|Cadeia de caracteres|UPN do usuário que criou esse recurso. Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|description|Cadeia de caracteres|A descrição do catálogo de pacotes de acesso.|
|displayName|Cadeia de caracteres|O nome de exibição do catálogo de pacotes de acesso.|
|id|String| Somente leitura.|
|isExternallyVisible|Booliano|Se os pacotes de acesso neste catálogo podem ser solicitados por usuários fora do locatário.|
|modifiedBy|Cadeia de caracteres|O UPN do usuário que modificou esse recurso pela última vez. Somente leitura.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |


## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackages|[Coleção accessPackage](accesspackage.md)| Os pacotes de acesso neste catálogo. Somente leitura. Anulável.|
|accessPackageResources|[Coleção accessPackageResource](accesspackageresource.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "keyProperty": "id"
}-->

```json
{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package catalog",
    "displayName":"Access package catalog for testing",
    "isExternallyVisible":false,
    "catalogType":"UserManaged",
    "catalogStatus":"Published",
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
  "description": "accessPackageCatalog resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

