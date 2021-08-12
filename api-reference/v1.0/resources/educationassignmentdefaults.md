---
title: Tipo de recurso educationAssignmentDefaults
description: Especifica os padrões de nível de classe respeitados por novas atribuições criadas na classe
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d9b9b624030129e85b2d89dc05db605af3cae7a4de72d019b41144a9453a23d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230764"
---
# <a name="educationassignmentdefaults-resource-type"></a>Tipo de recurso educationAssignmentDefaults

Namespace: microsoft.graph

Especifica os padrões de nível de classe respeitados por novas atribuições criadas na classe. 

Os chamadores podem continuar a especificar valores personalizados em cada criação de atribuição se não quiserem os comportamentos padrão.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter educationAssignmentDefaults](../api/educationassignmentdefaults-get.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|Leia as propriedades e as relações de um [objeto educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)|
|[Atualizar educationAssignmentDefaults](../api/educationassignmentdefaults-update.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|Atualize as propriedades de um [objeto educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|addedStudentAction|educationAddedStudentAction|Comportamento padrão no nível de classe para lidar com alunos que são adicionados após a publicação da atribuição. Os valores possíveis são: `none` e `assignIfOpen`.|
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
  "dueTime": "String (timestamp)",
  "notificationChannelUrl": "String"
}
```

