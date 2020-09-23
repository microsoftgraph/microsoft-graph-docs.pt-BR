---
title: tipo de recurso chatMessagePolicyViolation
description: Representa violação de política em uma mensagem de chat. As violações de política normalmente são definidas por um aplicativo DLP (prevenção de perda de dados).
author: laujan
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4ebe7acbb53793fdaac636e083b56f8acec36630
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223932"
---
# <a name="chatmessagepolicyviolation-resource-type"></a>tipo de recurso chatMessagePolicyViolation

Representa uma violação de política em uma mensagem de chat. As violações de política normalmente são definidas por um aplicativo DLP (prevenção de perda de dados). Os aplicativos DLP monitoram chats para mensagens que contêm dados que os usuários não devem enviar.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|dlpAction|**chatMessagePolicyViolationDlpActionType**|A ação executada pelo provedor de DLP na mensagem com conteúdo confidencial. Os valores compatíveis são: <li>Nenhum</li><li>NotifySender--informe o remetente da violação, mas permita que os leitores leiam a mensagem.</li><li>BlockAccess--impede que os leitores leiam a mensagem.</li><li>BlockAccessExternal--impede que os usuários de fora da organização leiam a mensagem, permitindo que os usuários dentro da organização leiam a mensagem.</li>|
|justificationText|string|Texto de justificativa fornecido pelo remetente da mensagem ao substituir uma violação de política.|
|policyTip|[chatMessagePolicyViolationPolicyTip](chatmessagepolicyviolationpolicytip.md)|Informações a serem exibidas para o remetente da mensagem sobre por que a mensagem foi sinalizada como uma violação. |
|UserAction|**chatMessagePolicyViolationUserActionType**|Indica a ação executada pelo usuário em uma mensagem bloqueada pelo provedor de DLP. Os valores compatíveis são: <li>Nenhum</li><li>Override</li><li>ReportFalsePositive</li>Quando o provedor de DLP está atualizando a mensagem para bloquear conteúdo confidencial, UserAction não é necessário.|
|verdictDetails|**chatMessagePolicyViolationVerdictDetailsType**|Indica quais ações o remetente pode executar em resposta à violação da política. Os valores compatíveis são: <li>Nenhum</li><li>AllowFalsePositiveOverride – permite que o remetente declare o policyViolation para ser um erro no aplicativo DLP e suas regras e permitir que os leitores vejam a mensagem novamente se o dlpAction tivesse ocultado.</li><li>AllowOverrideWithoutJustification – permite que o remetente fique superlado da violação de DLP e permita que os leitores vejam a mensagem novamente se o dlpAction tivesse ocultado, sem a necessidade de fornecer uma explicação para isso. </li><li>AllowOverrideWithJustification – permite que o remetente fique superlado da violação de DLP e permita que os leitores vejam a mensagem novamente se o dlpAction tivesse ocultado, depois de fornecer uma explicação para isso.</li>AllowOverrideWithoutJustification e AllowOverrideWithJustification são mutuamente exclusivos.|

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
