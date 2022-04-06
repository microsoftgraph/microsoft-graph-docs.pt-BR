---
title: Tipo de recurso membershipRuleProcessingStatus
description: Representa o status atual do processamento dinâmico do grupo.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 592a07abacf15300b25bfa00e9b477f9923d6c25
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64586906"
---
# <a name="membershipruleprocessingstatus-resource-type"></a>Tipo de recurso membershipRuleProcessingStatus

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status atual do processamento dinâmico do grupo.

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                                                                                   | Descrição                                                                                                                                                                |
| :-------------------- | :------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| status                | [membershipRuleProcessingStatusDetails](#membershipruleprocessingstatusdetails-values) | Status atual de um processamento dinâmico de grupo. Os valores possíveis são: `NotStarted`, `Running`, `Succeeded`, `Failed`e `UnknownFutureValue`. <br><br> Obrigatório. Somente leitura. |
| lastMembershipUpdated | edm. DateTime                                                                           | Data e hora mais recentes em que a associação de um grupo dinâmico foi atualizada. <br><br> Opcional. Somente leitura.                                                                    |
| errorMessage          | Cadeia de caracteres                                                                                 | Mensagem de erro detalhada se o processamento dinâmico de grupo ocorreu em um erro. <br><br> Opcional. Somente leitura.                                                                        |

### <a name="membershipruleprocessingstatusdetails-values"></a>membershipRuleProcessingStatusDetails values

| Member             | Descrição                                                                     |
| :----------------- | :------------------------------------------------------------------------------ |
| NotStarted         | O grupo foi criado ou atualizado e aguarda processamento.                     |
| Em execução            | O processamento foi iniciado.                                                         |
| Succeeded          | O processamento foi concluído. As alterações incrementais do objeto são processadas permanentemente. |
| Falhou             | O processamento ocorreu em um erro. Consulte **errorMessage** para obter detalhes.                 |
| UnknownFutureValue | Oferece suporte a valores futuros.                                                         |

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
