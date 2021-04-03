---
title: Tipo de recurso chatMessagePolicyViolation
description: Representa uma violação de política em uma mensagem de chat. As violações de política geralmente são definidas por um aplicativo de prevenção contra perda de dados (DLP).
author: RamjotSingh
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9c65b6dd1d07db43286a8cf9923f4a94f0855b34
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582267"
---
# <a name="chatmessagepolicyviolation-resource-type"></a>Tipo de recurso chatMessagePolicyViolation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma violação de política em uma mensagem de chat. As violações de política geralmente são definidas por um aplicativo de prevenção contra perda de dados (DLP). Os aplicativos DLP monitoram chats para mensagens que contêm dados que os usuários não devem enviar.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|dlpAction|**chatMessagePolicyViolationDlpActionType**|A ação realizada pelo provedor DLP na mensagem com conteúdo sensível. Os valores com suporte são: <li>Nenhum</li><li>NotifySender - Informe o remetente da violação, mas permita que os leitores leiam a mensagem.</li><li>BlockAccess - Impedir que os leitores leiam a mensagem.</li><li>BlockAccessExternal - Impedir que os usuários de fora da organização leiam a mensagem, permitindo que os usuários dentro da organização leiam a mensagem.</li>|
|justificationText|string|Texto de justificativa fornecido pelo remetente da mensagem ao se sobressuperar uma violação de política.|
|policyTip|[chatMessagePolicyViolationPolicyTip](chatmessagepolicyviolationpolicytip.md)|Informações a ser exibidas ao remetente da mensagem sobre o motivo pelo qual a mensagem foi sinalizada como uma violação. |
|userAction|**chatMessagePolicyViolationUserActionType**|Indica a ação tomada pelo usuário em uma mensagem bloqueada pelo provedor DLP. Os valores com suporte são: <li>Nenhum</li><li>Override</li><li>ReportFalsePositive</li>Quando o provedor de DLP está atualizando a mensagem para bloquear conteúdos confidenciais, userAction não é necessário.|
|verdictDetails|**chatMessagePolicyViolationVerdictDetailsType**|Indica quais ações o remetente pode tomar em resposta à violação da política. Os valores com suporte são: <li>Nenhum</li><li>AllowFalsePositiveOverride -- Permite que o remetente declare a políticaViolation como um erro no aplicativo DLP e suas regras e permita que os leitores vejam a mensagem novamente se a dlpAction a tiver ocultado.</li><li>AllowOverrideWithoutJustification -- permite que o remetente extravase a violação de DLP e permita que os leitores vejam a mensagem novamente se a dlpAction a tiver ocultado, sem a necessidade de fornecer uma explicação para fazer isso. </li><li>AllowOverrideWithJustification -- Permite que o remetente extravase a violação de DLP e permita que os leitores vejam a mensagem novamente se a dlpAction a tiver ocultado, depois de fornecer uma explicação para isso.</li>AllowOverrideWithoutJustification e AllowOverrideWithJustification são mutuamente exclusivos.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userAction",
    "justificationText"
  ],
  "@odata.type": "microsoft.graph.chatMessagePolicyViolation"
}-->

```json
{
  "dlpAction": "string",
  "justificationText": "string",
  "policyTip": {"@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip"},
  "userAction": "string",
  "verdictDetails": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message policy violation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
