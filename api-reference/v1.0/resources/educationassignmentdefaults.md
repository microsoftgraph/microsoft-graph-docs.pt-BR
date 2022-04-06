---
title: tipo de recurso educationAssignmentDefaults
description: Especifica padrões de nível de classe respeitados por novas atribuições criadas na classe
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 041cdef8dcdd81493882a7940d0505de94ad16eb
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684680"
---
# <a name="educationassignmentdefaults-resource-type"></a>tipo de recurso educationAssignmentDefaults

Namespace: microsoft.graph

Especifica padrões de nível de classe respeitados por novas atribuições criadas na classe. 

Os chamadores podem continuar especificando valores personalizados em cada criação de atribuição se não quiserem os comportamentos padrão.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter educationAssignmentDefaults](../api/educationassignmentdefaults-get.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|Leia as propriedades e as relações de um [objeto educationAssignmentDefaults](../resources/educationassignmentdefaults.md) .|
|[Atualizar educationAssignmentDefaults](../api/educationassignmentdefaults-update.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|Atualize as propriedades de [um objeto educationAssignmentDefaults](../resources/educationassignmentdefaults.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para educationAssignmentDefaults|
|addedStudentAction|educationAddedStudentAction|Comportamento padrão de nível de classe para lidar com alunos que são adicionados após a publicação da tarefa. Os valores possíveis são: `none` e `assignIfOpen`.|
|addToCalendarAction| educationAddToCalendarOptions|Campo opcional para controlar a adição de tarefas aos calendários dos alunos e professores quando a tarefa é publicada. Os valores possíveis são: `none`, `studentsAndPublisher`, `studentsAndTeamOwners`, `unknownFutureValue`e `studentsOnly`. Observe que você deve usar o `Prefer: include-unknown-enum-members` cabeçalho da solicitação para obter os seguintes valores nesta [enumeração evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `studentsOnly`. O valor padrão é `none`.|
|Duetime|TimeOfDay|Valor padrão de nível de classe para o campo de tempo devido. O valor padrão é `23:59:00`.|
|notificationChannelUrl|Cadeia de caracteres|Canal Teams padrão para o qual as notificações serão enviadas. O valor padrão é `null`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentDefaults",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "addedStudentAction": "String",
  "addToCalendarAction": "educationAddToCalendarOptions",  
  "dueTime": "String (timestamp)",
  "notificationChannelUrl": "String"
}
```

