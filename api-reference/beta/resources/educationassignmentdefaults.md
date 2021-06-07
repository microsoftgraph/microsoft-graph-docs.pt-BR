---
title: Tipo de recurso educationAssignmentDefaults
description: Especifica os padrões de nível de classe respeitados por novas atribuições criadas na classe
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: cdd4cb3814900f41f7cb7ee5ede407af61e9c4d7
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781062"
---
# <a name="educationassignmentdefaults-resource-type"></a>Tipo de recurso educationAssignmentDefaults

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica os padrões de nível de classe respeitados por novas atribuições criadas na classe. Os chamadores podem continuar a especificar valores personalizados em cada criação de atribuição se não quiserem os comportamentos padrão.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter educationAssignmentDefaults](../api/educationassignmentdefaults-get.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|Leia as propriedades e as relações de um [objeto educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)|
|[Atualizar educationAssignmentDefaults](../api/educationassignmentdefaults-update.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|Atualize as propriedades de um [objeto educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|addedStudentAction|educationAddedStudentAction|Comportamento padrão no nível de classe para lidar com alunos que são adicionados após a publicação da atribuição. Os valores possíveis são: `none` e `assignIfOpen`.|
|addToCalendarAction| educationAddToCalendarOptions|Campo opcional para controlar a adição de atribuições aos calendários dos alunos e professores quando a atribuição for publicada. Os valores possíveis são: `studentsAndPublisher`, `studentsAndTeamOwners`, `none`. O valor padrão é `none`.|
|dueTime|TimeOfDay|Valor padrão de nível de classe para o campo de tempo de vencimento. O valor padrão é `23:59:00`.|
|notificationChannelUrl|String|Canal Teams padrão para o qual as notificações serão enviadas. O valor padrão é `null`.|

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
  "addedStudentAction": "none",
  "addToCalendarAction": "none",
  "dueTime": "23:59:00",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
}
```

