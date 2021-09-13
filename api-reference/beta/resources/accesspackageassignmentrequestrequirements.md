---
title: Tipo de recurso accessPackageAssignmentRequestRequirements
description: Identifica os requisitos necessários para solicitar o pacote de acesso especificado.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5c30389c99ed550635e48713a1ad6fa449c66814
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057954"
---
# <a name="accesspackageassignmentrequestrequirements-resource-type"></a>Tipo de recurso accessPackageAssignmentRequestRequirements

Namespace: microsoft.graph

Representa os requisitos que um chamador deve atender para criar com êxito **um accessPackageAssignmentRequest** para **o accessPackage** especificado como parte da URL. Os requisitos são determinados pela avaliação de políticas associadas ao **accessPackage**. 

## <a name="properties"></a>Propriedades
| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| existingAnswers | [Coleção accessPackageAnswer](../resources/accesspackageanswer.md)  | Respostas que já foram fornecidas. |
| isApprovalRequired | Boleano | Indica se uma solicitação deve ser aprovada por um aprovador. |
| isApprovalRequiredForExtension  | Boleano | Indica se a aprovação é necessária quando um usuário tenta estender seu acesso. |
| isCustomAssignmentScheduleAllowed | Boleano | Indica se o solicitante tem permissão para definir uma agenda personalizada. |
| isRequestorJustificationRequired | Boleano | Indica se um solicitante deve fornecer justificativa ao enviar uma solicitação de atribuição. |
| policyDescription | Cadeia de Caracteres | A descrição da política que o usuário está tentando solicitar acesso usando.  |
| policyDisplayName | Cadeia de Caracteres | O nome de exibição da política que o usuário está tentando solicitar acesso usando. |
| policyId | Cadeia de Caracteres | O identificador da política à que esses requisitos estão associados. Esse identificador pode ser usado ao criar uma nova solicitação de atribuição. |
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
