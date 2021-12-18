---
title: Tipo de recurso educationAssignmentDefaults
description: Especifica os padrões de nível de classe respeitados por novas atribuições criadas na classe
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 620798d001df51bff352bcca4dce891a76f22cea
ms.sourcegitcommit: 15dd0e98e69f872ed5a709600608b244759b0967
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2021
ms.locfileid: "61567388"
---
# <a name="educationassignmentdefaults-resource-type"></a>Tipo de recurso educationAssignmentDefaults

Namespace: microsoft.graph

Especifica os padrões de nível de classe respeitados por novas atribuições criadas na classe. 

Os chamadores podem continuar a especificar valores personalizados em cada criação de atribuição se não quiserem os comportamentos padrão.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter educationAssignmentDefaults](../api/educationassignmentdefaults-get.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|Leia as propriedades e as relações de um [objeto educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)|
|[Atualizar educationAssignmentDefaults](../api/educationassignmentdefaults-update.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|Atualize as propriedades de um [objeto educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|addedStudentAction|educationAddedStudentAction|Comportamento padrão no nível de classe para lidar com alunos que são adicionados após a publicação da atribuição. Os valores possíveis são: `none` e `assignIfOpen`.|
|addToCalendarAction| educationAddToCalendarOptions|Campo opcional para controlar a adição de atribuições aos calendários dos alunos e professores quando a atribuição for publicada. Os valores possíveis são: `none` , , , e `studentsAndPublisher` `studentsAndTeamOwners` `unknownFutureValue` `studentsOnly` . Observe que você deve usar o header de solicitação para obter os seguintes valores nesta `Prefer: include-unknown-enum-members` [enum evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `studentsOnly` . O valor padrão é `none`.|
|dueTime|TimeOfDay|Valor padrão de nível de classe para o campo de tempo de vencimento. O valor padrão é `23:59:00`.|
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
  "addedStudentAction": "String",
  "addToCalendarAction": "educationAddToCalendarOptions",  
  "dueTime": "String (timestamp)",
  "notificationChannelUrl": "String"
}
```

