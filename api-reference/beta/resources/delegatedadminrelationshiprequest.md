---
title: Tipo de recurso delegatedAdminRelationshipRequest
description: Representa uma solicitação específica para uma relação de administrador delegado entre um parceiro e um cliente.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 5aaaabed54e6f5a4f0ba21cbdf64fb7d9deb0e8f
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821180"
---
# <a name="delegatedadminrelationshiprequest-resource-type"></a>Tipo de recurso delegatedAdminRelationshipRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma solicitação específica para uma relação de administrador delegado entre um parceiro e um cliente. Ele permite que o administrador de parceiros da Microsoft execute ações em uma relação, como bloquear uma relação para aprovação ou encerrar uma relação.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar delegatedAdminRelationshipRequest](../api/delegatedadminrelationship-post-requests.md)|[delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md)|Crie um novo **objeto delegatedAdminRelationshipRequest** .|
|[Listar delegatedAdminRelationshipRequests](../api/delegatedadminrelationship-list-requests.md)|[coleção delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md)|Obtenha uma lista dos **objetos delegatedAdminRelationshipRequest** e suas propriedades.|
|[Obter delegatedAdminRelationshipRequest](../api/delegatedadminrelationshiprequest-get.md)|[delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md)|Leia as propriedades e as relações de um **objeto delegatedAdminRelationshipRequest** .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|delegatedAdminRelationshipRequestAction|A ação a ser executada na relação de administrador delegado.|
|createdDateTime|DateTimeOffset|A data e hora no formato ISO 8601 e na hora UTC em que a solicitação de relação foi criada. Somente leitura. |
|id|Cadeia de caracteres|O identificador exclusivo da solicitação de relação. Somente leitura. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|A data e a hora no formato ISO 8601 e hora UTC em que essa solicitação de relação foi modificada pela última vez. Somente leitura.|
|status|delegatedAdminRelationshipRequestStatus|O status da solicitação. Somente leitura. Os valores possíveis são: `created`, `pending`, `succeeded`, `failed`, `unknownFutureValue`.|

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

