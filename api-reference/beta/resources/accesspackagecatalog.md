---
title: tipo de recurso accessPackageCatalog
description: Um catálogo de pacotes do Access é um contêiner para pacotes do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 66b7939541ba57dafc3be852c82c89781fc82381
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508531"
---
# <a name="accesspackagecatalog-resource-type"></a>tipo de recurso accessPackageCatalog

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure ad pretitulation Management](entitlementmanagement-root.md), um catálogo de pacotes do Access é um contêiner para zero ou mais pacotes de acesso.  Um catálogo de pacotes do Access também pode ter recursos vinculados que são usados nesses pacotes de acesso para fornecer acesso.


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageCatalogs](../api/accesspackagecatalog-list.md) | coleção [accessPackageCatalog](accesspackagecatalog.md) | Recupere uma lista de objetos accesspackagecatalog. |
| [Criar accessPackageCatalog](../api/accesspackagecatalog-post.md) | [accessPackageCatalog](accesspackagecatalog.md) | Criar um novo objeto accessPackageCatalog. |
| [Obter accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Ler propriedades e relações de um objeto accessPackageCatalog. |
| [Excluir accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | Exclua accessPackageCatalog. |
| [Listar recursos do accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresources.md) | coleção [accessPackageResource](accesspackageresource.md) | Recupere uma lista de objetos accessPackageResource em um catálogo. |
| [Listar funções de recurso accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | coleção [accessPackageResourceRole](accesspackageresourcerole.md) | Recupere uma lista de objetos accessPackageResourceRole para recursos em um catálogo. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|catalogStatus|String|Tem o valor `Published` se os pacotes de acesso estiverem disponíveis para gerenciamento.|
|CatalogType|String|Um `UserManaged` ou `ServiceDefault`. |
|createdBy|String|UPN do usuário que criou este recurso. Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|description|String|A descrição do catálogo de pacotes do Access.|
|displayName|Cadeia de caracteres|O nome de exibição do catálogo de pacotes do Access.|
|id|String| Somente leitura.|
|isExternallyVisible|Boolean|Se os pacotes de acesso neste catálogo podem ser solicitados por usuários fora do locatário.|
|modifiedBy|String|O UPN do usuário que modificou este recurso pela última vez. Somente leitura.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura. |


## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackages|coleção [accessPackage](accesspackage.md)| Os pacotes de acesso neste catálogo. Somente leitura. Anulável.|
|accessPackageResources|coleção [accessPackageResource](accesspackageresource.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "baseType": "",
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
