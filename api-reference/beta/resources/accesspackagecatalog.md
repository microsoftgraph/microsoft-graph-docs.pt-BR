---
title: Tipo de recurso accessPackageCatalog
description: Um catálogo de pacotes de acesso é um contêiner para pacotes de acesso.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2088bfea2aea6a8383b05826bf3783ea1a84de3f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63331865"
---
# <a name="accesspackagecatalog-resource-type"></a>Tipo de recurso accessPackageCatalog

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [gerenciamento de direitos do Azure AD](entitlementmanagement-overview.md), um catálogo de pacotes de acesso é um contêiner para zero ou mais pacotes de acesso. Um catálogo de pacotes de acesso também pode ter recursos vinculados usados nesses pacotes de acesso para fornecer acesso. Para exibir ou alterar a associação de funções com escopo de catálogo, use [a API de](unifiedroleassignment.md) atribuições de função com o provedor RBAC de gerenciamento de direitos.


## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageCatalogs](../api/entitlementmanagement-list-accesspackagecatalogs.md) | [Coleção accessPackageCatalog](accesspackagecatalog.md) | Recupere uma lista de objetos accesspackagecatalog. |
| [Criar accessPackageCatalog](../api/entitlementmanagement-post-accesspackagecatalogs.md) | [accessPackageCatalog](accesspackagecatalog.md) | Crie um novo objeto accessPackageCatalog. |
| [Obter accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Ler propriedades e relações de um objeto accessPackageCatalog. |
| [Atualizar accessPackageCatalog](../api/accesspackagecatalog-update.md)|Nenhum | Atualize as propriedades de um objeto accessPackageCatalog. |
| [Excluir accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | Exclua accessPackageCatalog. |
| **Recursos do pacote de acesso**| | |
| [Listar recursos do accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresources.md) | [Coleção accessPackageResource](accesspackageresource.md) | Recupere uma lista de objetos accessPackageResource em um catálogo. |
| **Funções de recurso do pacote de acesso**| | |
| [Listar funções de recurso accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [Coleção accessPackageResourceRole](accesspackageresourcerole.md) | Recupere uma lista de objetos accessPackageResourceRole para recursos em um catálogo. |
| **Extensões de fluxo de trabalho do pacote de pacote de acesso personalizado**| | |
|[Listar customAccessPackageWorkflowExtensions](../api/accesspackagecatalog-list-customaccesspackageworkflowextensions.md)|[coleção customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Obter uma lista dos [objetos customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) e suas propriedades.|
|[Criar customAccessPackageWorkflowExtensions](../api/accesspackagecatalog-post-customaccesspackageworkflowextensions.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Crie um novo [objeto customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|
|[Obter customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-get.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Leia as propriedades e as relações de um [objeto customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|
|[Atualizar customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-update.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Atualize as propriedades de [um objeto customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|
|[Excluir customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-delete.md)|Nenhum(a)|Exclui um [objeto customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) .|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|catalogStatus|String|Tem o valor `Published` se os pacotes de acesso estão disponíveis para gerenciamento.|
|catalogType|String|Um de `UserManaged` ou `ServiceDefault`. |
|createdBy|Cadeia de caracteres|UPN do usuário que criou esse recurso. Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|description|String|A descrição do catálogo de pacotes de acesso.|
|displayName|String|O nome de exibição do catálogo de pacotes de acesso. Suporta `$filter` (`eq`, `contains`).|
|id|String| Somente leitura.|
|isExternallyVisible|Booliano|Se os pacotes de acesso neste catálogo podem ser solicitados por usuários fora do locatário.|
|modifiedBy|String|O UPN do usuário que modificou esse recurso pela última vez. Somente leitura.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |


## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackages|[Coleção accessPackage](accesspackage.md)| Os pacotes de acesso neste catálogo. Somente leitura. Anulável. Suporta o `$expand`.|
|accessPackageResources|[Coleção accessPackageResource](accesspackageresource.md)| Somente leitura. Anulável.|
|accessPackageResourceRoles|[Coleção accessPackageResourceRole](accesspackageresourcerole.md)|As funções em cada recurso em um catálogo. Somente leitura.|
|accessPackageResourceScopes|[Coleção accessPackageResourceScope](accesspackageresourcescope.md)|Somente leitura.|
|customAccessPackageWorkflowExtension|[coleção customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Os atributos de um aplicativo lógico, que pode ser chamado em vários estágios de um ciclo de solicitação e atribuição de pacote de acesso. |

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

