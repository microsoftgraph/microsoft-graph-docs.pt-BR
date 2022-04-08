---
title: Tipo de recurso delegatedAdminAccessAssignment
description: Representa uma atribuição de funções administrativas ao contêiner de acesso de um parceiro da Microsoft.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: a9d831325d211233062d93ce1ccda1128d9dfb4b
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704335"
---
# <a name="delegatedadminaccessassignment-resource-type"></a>Tipo de recurso delegatedAdminAccessAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma atribuição de funções administrativas a um parceiro da Microsoft usando a administração delegada. As funções administrativas são atribuídas ao parceiro da Microsoft por meio de um contêiner de acesso (como um grupo de segurança). Quando ele estiver ativo, os membros do contêiner de acesso obterão acesso às funções especificadas nos detalhes de acesso.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar delegatedAdminAccessAssignment](../api/delegatedadminrelationship-post-accessassignments.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|Crie um novo **objeto delegatedAdminAccessAssignment** .|
|[Listar delegatedAdminAccessAssignments](../api/delegatedadminrelationship-list-accessassignments.md)|[coleção delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|Obtenha uma lista dos **objetos delegatedAdminAccessAssignment** e suas propriedades.|
|[Obter delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-get.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|Leia as propriedades e as relações de um **objeto delegatedAdminAccessAssignment** .|
|[Atualizar delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-update.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|Atualize as propriedades de **um objeto delegatedAdminAccessAssignment** .|
|[Excluir delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-delete.md)|Nenhum|**Exclua um objeto delegatedAdminAccessAssignment**.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accessContainer|[delegatedAdminAccessContainer](../resources/delegatedadminaccesscontainer.md)|O contêiner de acesso por meio do qual os membros recebem acesso. Por exemplo, um grupo de segurança.|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|Os detalhes de acesso que contêm os identificadores das funções administrativas atribuídas pelo parceiro no locatário do cliente.|
|createdDateTime|DateTimeOffset|A data e a hora no formato ISO 8601 e na hora UTC em que a atribuição de acesso foi criada. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo da atribuição de acesso. Somente leitura. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|A data e a hora no ISO 8601 e na hora UTC em que essa atribuição de acesso foi modificada pela última vez. Somente leitura.|
|status|delegatedAdminAccessAssignmentStatus|O status da atribuição de acesso. Somente leitura. Os valores possíveis são: `pending`, `active`, `deleting`, `deleted`, `error`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.delegatedAdminAccessAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminAccessAssignment",
  "id": "String (identifier)",
  "status": "String",
  "accessContainer": {
    "@odata.type": "microsoft.graph.delegatedAdminAccessContainer"
  },
  "accessDetails": {
    "@odata.type": "microsoft.graph.delegatedAdminAccessDetails"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

