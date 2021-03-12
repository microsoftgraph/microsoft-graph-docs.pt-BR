---
title: Tipo de recurso conditionalAccessPolicy
description: Representa uma política de acesso condicional do Azure Active Directory. As políticas de acesso condicional são regras personalizadas que definem um cenário de acesso.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: bbb38453015f1b00b9a290913eeb9c03a090b045
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721548"
---
# <a name="conditionalaccesspolicy-resource-type"></a>Tipo de recurso conditionalAccessPolicy

Namespace: microsoft.graph

Representa uma política de acesso condicional do Azure Active Directory. As políticas de acesso condicional são regras personalizadas que definem um cenário de acesso. Para obter mais informações, consulte [a documentação de acesso condicional](/azure/active-directory/conditional-access/).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar conditionalAccessPolicies](../api/conditionalaccessroot-list-policies.md) | [conditionalAccessPolicy](conditionalaccesspolicy.md) conjunto | Obter todos os objetos conditionalAccessPolicies na organização. |
| [Criar conditionalAccessPolicy](../api/conditionalaccessroot-post-policies.md) | [conditionalAccessPolicy](conditionalaccesspolicy.md) | Crie um novo objeto conditionalAccessPolicy. |
| [Obter conditionalAccessPolicy](../api/conditionalaccesspolicy-get.md) | [conditionalAccessPolicy](conditionalaccesspolicy.md) | Ler propriedades e relações de um objeto conditionalAccessPolicy. |
| [Atualizar conditionalAccessPolicy](../api/conditionalaccesspolicy-update.md) | [conditionalAccessPolicy](conditionalaccesspolicy.md) | Atualize um objeto conditionalAccessPolicy. |
| [Excluir conditionalAccessPolicy](../api/conditionalaccesspolicy-delete.md) | Nenhum | Exclua um objeto conditionalAccessPolicy. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|conditions|[conditionalAccessConditionSet](conditionalaccessconditionset.md)| Especifica as regras que devem ser atendidas para que a política seja aplicada. Obrigatório. |
|createdDateTime|DateTimeOffset| O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Readonly. |
|displayName|Cadeia de caracteres| Especifica um nome de exibição para o objeto conditionalAccessPolicy. |
|grantControls|[conditionalAccessGrantControls](conditionalaccessgrantcontrols.md)| Especifica os controles de concessão que devem ser cumpridos para passar a política. |
|id|Cadeia de caracteres| Especifica o identificador de um objeto conditionalAccessPolicy. Somente leitura.|
|modifiedDateTime| DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Readonly. |
|sessionControls|[conditionalAccessSessionControls](conditionalaccesssessioncontrols.md)| Especifica os controles de sessão que são imposto após a assinatura. |
|estado|string| Especifica o estado do objeto conditionalAccessPolicy. Os valores possíveis são: `enabled`, `disabled`, `enabledForReportingButNotEnforced`. Obrigatório. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy",
  "keyProperty": "id"
}-->

```json
{
  "conditions": {"@odata.type": "microsoft.graph.conditionalAccessConditionSet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "grantControls": {"@odata.type": "microsoft.graph.conditionalAccessGrantControls"},
  "id": "String (identifier)",
  "modifiedDateTime": "String (timestamp)",
  "sessionControls": {"@odata.type": "microsoft.graph.conditionalAccessSessionControls"},
  "state": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
