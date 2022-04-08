---
title: Tipo de recurso delegatedAdminRelationshipOperation
description: Representa uma operação de execução longa relacionada a uma relação de administrador delegado.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 9eef6d0de67b3e124f95cd0763ac5948b6d2fd10
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704158"
---
# <a name="delegatedadminrelationshipoperation-resource-type"></a>Tipo de recurso delegatedAdminRelationshipOperation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma operação de execução longa relacionada a uma relação de administrador delegado. Um exemplo de uma operação de execução longa pode ser uma atualização para o objeto [delegatedAdminAccessAssignment](delegatedAdminAccessAssignment.md) .

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar delegatedAdminRelationshipOperations](../api/delegatedadminrelationship-list-operations.md)|[coleção delegatedAdminRelationshipOperation](delegatedadminrelationshipoperation.md)|Obtenha uma lista dos **objetos delegatedAdminRelationshipOperation** e suas propriedades.|
|[Obter delegatedAdminRelationshipOperation](../api/delegatedadminrelationshipoperation-get.md)|[delegatedAdminRelationshipOperation](delegatedadminrelationshipoperation.md)|Leia as propriedades e as relações de um **objeto delegatedAdminRelationshipOperation** .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|A hora no formato ISO 8601 e no horário UTC em que a operação de execução longa foi criada. Somente leitura.|
|data|Cadeia de caracteres|Os dados (conteúdo) da operação. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo da operação de execução longa do administrador delegado. Somente leitura. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|A hora no formato ISO 8601 e no horário UTC em que a operação de execução longa foi modificada pela última vez. Somente leitura.|
|operationType|delegatedAdminRelationshipOperationType|O tipo de operação de execução longa. Os valores possíveis são: `delegatedAdminAccessAssignmentUpdate`, `unknownFutureValue`. Somente leitura.|
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
