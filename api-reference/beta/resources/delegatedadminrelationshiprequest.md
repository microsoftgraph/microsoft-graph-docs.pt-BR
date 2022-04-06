---
title: tipo de recurso delegatedAdminRelationshipRequest
description: Representa uma solicitação específica de uma relação de administrador delegada entre um parceiro e um cliente.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 7381f4acf3ec04f4bdf4ef8f3a8bdf3744efa81d
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589532"
---
# <a name="delegatedadminrelationshiprequest-resource-type"></a>tipo de recurso delegatedAdminRelationshipRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma solicitação específica de uma relação de administrador delegada entre um parceiro e um cliente. Ele permite que o administrador do parceiro da Microsoft tome ações em um relacionamento, como bloquear uma relação para aprovação ou encerrar um relacionamento.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar delegatedAdminRelationshipRequest](../api/delegatedadminrelationship-post-requests.md)|[delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md)|Crie um novo **objeto delegatedAdminRelationshipRequest** .|
|[Listar delegatedAdminRelationshipRequests](../api/delegatedadminrelationship-list-requests.md)|[coleção delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md)|Obter uma lista dos **objetos delegatedAdminRelationshipRequest** e suas propriedades.|
|[Obter delegatedAdminRelationshipRequest](../api/delegatedadminrelationshiprequest-get.md)|[delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md)|Leia as propriedades e as relações de um **objeto delegatedAdminRelationshipRequest** .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|delegatedAdminRelationshipRequestAction|A ação a ser executada na relação de administrador delegada.|
|createdDateTime|DateTimeOffset|A data e a hora no formato ISO 8601 e no horário UTC quando a solicitação de relação foi criada. Somente leitura. |
|id|Cadeia de caracteres|O identificador exclusivo da solicitação de relação. Somente leitura. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|A data e a hora no formato ISO 8601 e a hora UTC quando essa solicitação de relação foi modificada pela última vez. Somente leitura.|
|status|delegatedAdminRelationshipRequestStatus|O status da solicitação. Somente leitura. Os valores possíveis são: `created`, `pending`, `complete`, `failed`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedAdminRelationshipRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationshipRequest",
  "id": "String (identifier)",
  "action": "String",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

