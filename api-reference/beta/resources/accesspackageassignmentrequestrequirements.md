---
title: Tipo de recurso accessPackageAssignmentRequestRequirements
description: Identifica os requisitos necessários para solicitar o pacote de acesso especificado.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: febe429bb3c29da1a58454bb2758ee0fae16735b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259199"
---
# <a name="accesspackageassignmentrequestrequirements-resource-type"></a>Tipo de recurso accessPackageAssignmentRequestRequirements

Namespace: microsoft.graph

Representa os requisitos que um chamador deve atender para criar com êxito **um accessPackageAssignmentRequest** para **o accessPackage** especificado como parte da URL. Os requisitos são determinados pela avaliação de políticas associadas ao **accessPackage**. 

## <a name="properties"></a>Propriedades
| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| existingAnswers | [Coleção accessPackageAnswer](../resources/accesspackageanswer.md)  | Respostas que já foram fornecidas. |
| isApprovalRequired | Boolean | Indica se uma solicitação deve ser aprovada por um aprovador. |
| isApprovalRequiredForExtension  | Boolean | Indica se a aprovação é necessária quando um usuário tenta estender seu acesso. |
| isCustomAssignmentScheduleAllowed | Boolean | Indica se o solicitante tem permissão para definir uma agenda personalizada. |
| isRequestorJustificationRequired | Boolean | Indica se um solicitante deve fornecer justificativa ao enviar uma solicitação de atribuição. |
| policyDescription | Cadeia de caracteres | A descrição da política que o usuário está tentando solicitar acesso usando.  |
| policyDisplayName | Cadeia de caracteres | O nome de exibição da política que o usuário está tentando solicitar acesso usando. |
| policyId | Cadeia de caracteres | O identificador da política à que esses requisitos estão associados. Esse identificador pode ser usado ao criar uma nova solicitação de atribuição. |
| questions | [Coleção accessPackageQuestion](../resources/accesspackagequestion.md) | Perguntas configuradas na política. As perguntas podem ser necessárias ou opcionais; os chamadores podem determinar se uma pergunta é necessária ou opcional com base na **propriedade isRequired** em **accessPackageQuestion**. |
| Cronograma | [requestSchedule](../resources/requestschedule.md) | Restrições de agendamento impostas, se alguma. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON do tipo.

<!-- { 
  "blockType": "resource", 
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequestRequirements" 
}-->

``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequestRequirements",
  "policyId": "String",
  "policyDisplayName": "String",
  "policyDescription": "String",
  "isApprovalRequired": false,
  "isApprovalRequiredForExtension": false,
  "isCustomAssignmentScheduleAllowed": false,
  "isRequestorJustificationRequired": false,
  "schedule": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "questions": [
    {
      "@odata.type": "microsoft.graph.accessPackageQuestion"
    }
  ],
  "existingAnswers": [
    {
      "@odata.type": "microsoft.graph.accessPackageAnswerString"
    }
  ]
}
```
