---
title: tipo de recurso trialBalance
description: Um objeto de balancete no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1a7e906e50ddf39e4c9e2d3d9dde11226c7ec662
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534847"
---
# <a name="trialbalance-resource-type"></a>tipo de recurso trialBalance
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

