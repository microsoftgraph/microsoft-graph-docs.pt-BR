---
title: Tipo de recurso unifiedRoleAssignment
description: Uma atribuição de função é o link entre uma definição de função e uma entidade principal em um escopo específico para a finalidade de conceder acesso.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: fd6323fa0eb99f440551916cbc535fa64a359275
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148496"
---
# <a name="unifiedroleassignment-resource-type"></a>Tipo de recurso unifiedRoleAssignment

Namespace: microsoft.graph

Uma atribuição de função é usada para conceder acesso aos recursos. Representa uma definição de função atribuída a uma entidade principal (por exemplo, um usuário ou um grupo atribuível a função) em um escopo específico.

Herda da [entidade](entity.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[Listar unifiedRoleAssignments](../api/rbacapplication-list-roleassignments.md)|[Coleção unifiedRoleAssignment](../resources/unifiedroleassignment.md)| Obter uma lista dos [objetos unifiedRoleAssignment](../resources/unifiedroleassignment.md) e suas propriedades.|
|[Criar unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|Crie um novo [objeto unifiedRoleAssignment.](../resources/unifiedroleassignment.md)|
|[Obter unifiedRoleAssignment](../api/unifiedroleassignment-get.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|Leia as propriedades e as relações de um [objeto unifiedRoleAssignment.](../resources/unifiedroleassignment.md)|
|[Excluir unifiedRoleAssignment](../api/unifiedroleassignment-delete.md)|Nenhum(a)|Exclui um [objeto unifiedRoleAssignment.](../resources/unifiedroleassignment.md)|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| O identificador exclusivo da atribuição de função. Chave, não anulada, somente leitura. Herdado da [entidade](entity.md).|
|roleDefinitionId|Cadeia de caracteres| Identificador da definição de função para a atribuição. Somente leitura. Suporta $filter ( `eq` , `in` ).|
|principalId|Cadeia de caracteres| Identificador da entidade à qual a atribuição é concedida. Suporta $filter ( `eq` , `in` ).|
|directoryScopeId|String|Identificador do objeto directory que representa o escopo da atribuição.  Essa propriedade ou **appScopeId** é necessária. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. Suporta $filter ( `eq` , `in` ).|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando o escopo de atribuição for específico do aplicativo.  Essa propriedade ou **directoryScopeId** é obrigatório. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. Use `/` para escopos de aplicativos de todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. Suporta $filter ( `eq` , `in` ).|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|principal|[directoryObject](directoryobject.md)| Fazendo referência à entidade atribuída. Somente leitura. Oferece suporte para `$expand`.|
|roleDefinition|[unifiedRoleDefinition](unifiedroledefinition.md)|A funçãoDefinition para a atribuição.  Suporta o `$expand`. roleDefinition.Id será expandido automaticamente.
|directoryScope|[directoryObject](directoryobject.md)|O objeto directory que é o escopo da atribuição. Somente leitura. Oferece suporte para `$expand`.|
|appScope|[appScope](appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção. Suporta o `$expand`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
  "id": "String (identifier)",
  "appScopeId": "String",
  "condition": "String",
  "directoryScopeId": "String",
  "principalId": "String",
  "roleDefinitionId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
