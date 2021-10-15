---
title: tipo de recurso meetingRegistration
description: Contém informações sobre o registro de reunião online.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 87a9f71d44df2610021c0cc93aa42fc080d3f8d4
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/15/2021
ms.locfileid: "60370319"
---
# <a name="meetingregistration-resource-type"></a>tipo de recurso meetingRegistration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes do registro de uma reunião online, como um [Microsoft Teams Webinar](https://support.microsoft.com/en-us/office/get-started-with-teams-webinars-42f3f874-22dc-4289-b53f-bbc1a69013e3).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
| :----- | :---------- | :---------- |
|[Criar](../api/meetingregistration-post.md) | [meetingRegistration](meetingregistration.md) | Criar e habilitar o registro para uma reunião online. |
|[Obter](../api/meetingregistration-get.md) | [meetingRegistration](meetingregistration.md) | Recupere os detalhes de um registro de reunião. |
|[Atualizar](../api/meetingregistration-update.md) | [meetingRegistration](meetingregistration.md) | Atualize os detalhes de um registro de reunião. |
|[Excluir](../api/meetingregistration-delete.md) | [meetingRegistration](meetingregistration.md) | Desabilitar e excluir o registro de uma reunião online. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
| :------- | :--- | :---------- |
| allowedRegistrant | [meetingAudience](#meetingaudience-values) | Especifica quem pode se registrar na reunião. |
| description | Cadeia de caracteres | A descrição da reunião. |
| endDateTime | DateTime | A hora de término da reunião em UTC. |
| registrationPageViewCount | Int32 | O número de vezes que a página de registro foi visitada. Apenas leitura. |
| registrationPageWebUrl | Cadeia de caracteres | A URL da página de registro. Apenas leitura. |
| falantes | [Coleção meetingSpeaker](meetingSpeaker.md) | As informações do orador da reunião. |
| startDateTime | DateTime | O horário de início da reunião em UTC. |
| assunto | Cadeia de caracteres | O assunto da reunião. |

### <a name="meetingaudience-values"></a>valores meetingAudience

| Valor              | Descrição |
| ------------------ | ----------- |
| everyone           | Todos podem se registrar na reunião. |
| organização       | Todos na organização do organizador podem se registrar na reunião. |
| unknownFutureValue | Valor de sentinela de enumeração evolvável. Não usar. |

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
| ------------ | ---- | ----------- |
| customQuestions | [coleção meetingRegistrationQuestion](meetingRegistrationQuestion.md)| Perguntas de registro personalizadas. |
| registrants | [coleção meetingRegistrant](meetingRegistrant.md) | Registrantes da reunião online. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingRegistration"
}-->

```json
{
  "allowedRegistrant": { "@odata.type": "microsoft.graph.meetingAudience" },
  "description": "String",
  "endDateTime": "String (timestamp)",
  "registrationPageViewCount": "Int32",
  "registrationPageWebUrl": "String",
  "speakers": [{ "@odata.type": "microsoft.graph.meetingSpeaker" }],
  "startDateTime": "String (timestamp)",
  "subject": "String",

  "customQuestions": [{ "@odata.type": "microsoft.graph.meetingRegistrationQuestion" }],
  "registrants": [{ "@odata.type": "microsoft.graph.meetingRegistrant" }]
}
```
