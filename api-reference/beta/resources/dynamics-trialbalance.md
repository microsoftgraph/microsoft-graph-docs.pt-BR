---
title: tipo de recurso trialBalance
description: Um objeto de balancete no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 43368ace9a47064833aa388dda0a7da31d9e5f0c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040032"
---
# <a name="trialbalance-resource-type"></a>tipo de recurso trialBalance

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um balancete no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter trialBalance](../api/dynamics-trialbalance-get.md)|trialBalance|Obtém um objeto de saldo de avaliação.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|number|string|O número da conta de G/L do item trialBalance|
|accountId|GUID|O identificador exclusivo da conta de G/L do registro.|
|accountType|string|O tipo de conta da conta G/L do registro.|
|Exiba|string|O nome da conta do G/L para o item trialBalance.|
|totalDebit|string|Representa o valor total de débito na conta G/L.|
|totalCredit|string|Representa o valor total de crédito na conta G/L.|
|balanceAtDateDebit|string|Representa o saldo positivo no valor da data na conta G/L.|
|balanceAtDateCredit|string|Representa o saldo negativo no valor da data na conta G/L.|
|dateFilter|data|O filtro de data usado para calcular os itens do trialBalance.|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


```json
{
    "number": "string",
    "accountId": "GUID",
    "accountType": "string",
    "display": "string",
    "totalDebit": "string",
    "totalCredit": "string",
    "balanceAtDateDebit": "string",
    "balanceAtDateCredit": "string",
    "dateFilter": "date"
}

```



