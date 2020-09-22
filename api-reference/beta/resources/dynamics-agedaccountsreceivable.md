---
title: tipo de recurso agedAccountsReceivable
description: Um objeto de contas a receber antiga no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 4d56e954e39bae22db07e025f9570f1fe7a92280
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040053"
---
# <a name="agedaccountsreceivable-resource-type"></a>tipo de recurso agedAccountsReceivable

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um objeto agedAccountsReceivable no Dynamics 365 Business central, que está mostrando o envelhecimento de uma conta de cliente.

## <a name="methods"></a>Métodos

| Método         | Tipo de retorno  |Descrição|
|:---------------|:-------------|:----------|
|[Obter agedAccountsReceivable](../api/dynamics-agedaccountsreceivable-get.md)|agedAccountsReceivable|Obter o objeto agedAccountsReceivable|

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo    |Descrição                                  |
|:---------------|:--------|:--------------------------------------------|
|Box      |GUID     |A ID exclusiva do cliente.                   |
|customerNumber  |string   |Especifica o número do cliente.                 |
|nome            |string   |Especifica o nome do cliente.                   |
|currencyCode    |string   |Especifica a moeda.                      |
|balanceDue      |numéricos  |Especifica o saldo total do cliente.      |
|currentAmount   |numéricos  |Especifica o saldo para o período de envelhecimento atual.|
|period1Amount   |numéricos  |Especifica o saldo no primeiro período de classificação por vencimento. |
|period2Amount   |numéricos  |Especifica o saldo no segundo período de envelhecimento.|
|period3Amount   |numéricos  |Especifica o saldo no terceiro período de envelhecimento. |
|agedAsOfDate    |data     |Especifica a data de início do período usada para calcular os períodos de expiração.|
|periodLengthFilter|string |Especifica o comprimento dos períodos. As unidades de tempo aceitáveis incluem: D, WD, W, M, Q e Y. C, o que significa a unidade de tempo atual com base na data, pode ser especificada como um prefixo para a unidade de tempo.|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


```json
{
    "customerId": "GUID",
    "customerNumber": "string",
    "name": "string",
    "currencyCode": "string",
    "balanceDue": "decimal",
    "currentAmount": "decimal",
    "period1Amount": "decimal",
    "period2Amount": "decimal",
    "period3Amount": "decimal",
    "agedAsOfDate": "date",
    "periodLengthFilter": "string"
}

```




