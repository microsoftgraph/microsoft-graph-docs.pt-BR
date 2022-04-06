---
title: tipo de recurso delegatedAdminAccessAssignment
description: Representa uma atribuição de funções administrativas para um contêiner de acesso do parceiro Microsoft.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: eec8597ffa629b919a7f9b7a9f9d22fbdcde2217
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589554"
---
# <a name="delegatedadminaccessassignment-resource-type"></a>tipo de recurso delegatedAdminAccessAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma atribuição de funções administrativas a um parceiro da Microsoft usando a administração delegada. As funções administrativas são atribuídas ao parceiro microsoft por meio de um contêiner de acesso (como um grupo de segurança). Quando ele está ativo, os membros do contêiner de acesso têm acesso às funções especificadas nos detalhes de acesso.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar delegatedAdminAccessAssignment](../api/delegatedadminrelationship-post-accessassignments.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|Crie um novo **objeto delegatedAdminAccessAssignment** .|
|[Listar delegatedAdminAccessAssignments](../api/delegatedadminrelationship-list-accessassignments.md)|[coleção delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|Obter uma lista dos **objetos delegatedAdminAccessAssignment** e suas propriedades.|
|[Obter delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-get.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|Leia as propriedades e as relações de um **objeto delegatedAdminAccessAssignment** .|
|[Atualizar delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-update.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|Atualize as propriedades de um **objeto delegatedAdminAccessAssignment** .|
|[Excluir delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-delete.md)|Nenhum|**Exclua um objeto delegatedAdminAccessAssignment**.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accessContainer|[delegatedAdminAccessContainer](../resources/delegatedadminaccesscontainer.md)|O contêiner de acesso pelo qual os membros são atribuídos acesso. Por exemplo, um grupo de segurança.|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|Os detalhes de acesso que contêm os identificadores das funções administrativas atribuídas ao parceiro no locatário do cliente.|
|createdDateTime|DateTimeOffset|A data e a hora no formato ISO 8601 e no horário UTC quando a atribuição de acesso foi criada. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo da atribuição de acesso. Somente leitura. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|A data e a hora na ISO 8601 e no horário UTC quando essa atribuição de acesso foi modificada pela última vez. Somente leitura.|
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

