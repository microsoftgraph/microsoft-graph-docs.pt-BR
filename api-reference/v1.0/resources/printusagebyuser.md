---
title: Tipo de recurso printUsageByUser
description: Descreve a atividade de impressão de um usuário durante um período de tempo especificado (usageDate).
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: f702c0dcb81d1b88f2c9bb0e314e74b97a905004
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60936100"
---
# <a name="printusagebyuser-resource-type"></a>Tipo de recurso printUsageByUser

Namespace: microsoft.graph

Descreve a atividade de impressão de um usuário durante um período de tempo especificado (usageDate).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Lista (diariamente)](../api/reportroot-list-dailyprintusagebyuser.md) | [printUsageByUser](printusagebyuser.md) | Obter uma lista de resumos de uso diário de impressão, agrupados por usuário. |
| [Lista (mensal)](../api/reportroot-list-monthlyprintusagebyuser.md) | [printUsageByUser](printusagebyuser.md) | Obter uma lista de resumos de uso de impressão mensal, agrupados por usuário. |
| [Get](../api/printusagebyuser-get.md) | [printUsageByUser](printusagebyuser.md) | Ler propriedades e relações de um objeto printUsageByUser. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID deste resumo de uso.|
|userPrincipalName|Cadeia de caracteres|O UPN do usuário representado por essas estatísticas.|
|usageDate|Data|A data associada a essas estatísticas.|
|completedBlackAndWhiteJobCount|Int64|O número de trabalhos de impressão em preto e branco concluídos em nome do usuário na data associada.|
|completedColorJobCount|Int64|O número de trabalhos de impressão de cores concluídos em nome do usuário na data associada.|
|incompleteJobCount|Int64|O número de trabalhos de impressão que foram enraizadas em nome do usuário, mas não concluídos, na data associada.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printUsageByUser",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printUsageByUser",
  "id": "String (identifier)",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer",
  "userPrincipalName": "String"
}
```

