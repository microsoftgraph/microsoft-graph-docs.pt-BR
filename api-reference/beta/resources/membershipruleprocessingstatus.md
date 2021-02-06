---
title: Tipo de recurso membershipRuleProcessingStatus
description: Representa o status atual do processamento de grupo dinâmico.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: f59f5f89c3aad8312504c62b29a0dbd490a37ac5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128257"
---
# <a name="membershipruleprocessingstatus-resource-type"></a>Tipo de recurso membershipRuleProcessingStatus

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status atual do processamento de grupo dinâmico.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| status | [membershipRuleProcessingStatusDetails](#membershipruleprocessingstatusdetails-values) | Status atual de um processamento de grupo dinâmico. Os valores possíveis `NotStarted` são: `Running` , , e `Succeeded` `Failed` `UnknownFutureValue` .  <br><br> Obrigatório. Somente leitura.|
| lastMembershipUpdated | edm. DateTime | Data e hora mais recentes quando a associação de um grupo dinâmico foi atualizada. <br><br> Opcional. Somente leitura.|
| errorMessage | String | Mensagem de erro detalhada se o processamento de grupo dinâmico encontrou um erro. <br><br> Opcional. Somente leitura.|

### <a name="membershipruleprocessingstatusdetails-values"></a>Valores de membershipRuleProcessingStatusDetails

| Member | Descrição |
|:-------- |:----------- |
| NotStarted | O grupo foi criado ou atualizado e aguardando processamento.|
| Em execução | O processamento foi iniciado.|
| Succeeded | O processamento foi concluído. As alterações incrementais de objeto são processadas permanentemente. |
| Falhou | O processamento encontrou um erro. Consulte **errorMessage** para obter detalhes. |
| UnknownFutureValue | Oferece suporte a valores futuros. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.membershipRuleProcessingStatus",
  "baseType": null
}-->

```json
{
  "status": "string",
  "lastMembershipUpdated": "DateTime",
  "errorMessage": "string"
}
```
