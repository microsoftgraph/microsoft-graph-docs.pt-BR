---
title: Tipo de recurso delegatedAdminRelationshipOperation
description: Representa uma operação de longa duração relacionada a uma relação de administrador delegada.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 50aaad489ba955c4d7ba2a9c0992e63b445732b5
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589533"
---
# <a name="delegatedadminrelationshipoperation-resource-type"></a>Tipo de recurso delegatedAdminRelationshipOperation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma operação de longa duração relacionada a uma relação de administrador delegada. Um exemplo de uma operação de longa duração pode ser uma atualização para o [objeto delegatedAdminAccessAssignment](delegatedAdminAccessAssignment.md) .

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar delegatedAdminRelationshipOperations](../api/delegatedadminrelationship-list-operations.md)|[coleção delegatedAdminRelationshipOperation](delegatedadminrelationshipoperation.md)|Obter uma lista dos **objetos delegatedAdminRelationshipOperation** e suas propriedades.|
|[Obter delegatedAdminRelationshipOperation](../api/delegatedadminrelationshipoperation-get.md)|[delegatedAdminRelationshipOperation](delegatedadminrelationshipoperation.md)|Leia as propriedades e as relações de um **objeto delegatedAdminRelationshipOperation** .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|O tempo no formato ISO 8601 e no horário UTC em que a operação de longa duração foi criada. Somente leitura.|
|data|Cadeia de caracteres|Os dados (carga) da operação. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo da operação de longa duração do administrador delegado. Somente leitura. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|O tempo no formato ISO 8601 e no horário UTC em que a operação de longa duração foi modificada pela última vez. Somente leitura.|
|operationType|delegatedAdminRelationshipOperationType|O tipo de operação de longa duração. Os valores possíveis são: `delegatedAdminAccessAssignmentUpdate`, `unknownFutureValue`. Somente leitura.|
|status|delegatedAdminRelationshipOperationStatus|O status da operação. Somente leitura. Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`. Somente leitura. Oferece suporte para `$orderBy`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedAdminRelationshipOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationshipOperation",
  "id": "String (identifier)",
  "operationType": "String",
  "data": "String",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```
