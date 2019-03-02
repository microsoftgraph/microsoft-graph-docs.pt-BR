---
title: tipo de recurso agedAccountsPayable
description: Um objeto de contas a pagar antigo no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 679c24b7ef32ef59b34a5885ea745d8c244376b2
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365903"
---
# <a name="agedaccountspayable-resource-type"></a>tipo de recurso agedAccountsPayable
Representa um objeto agedAccountsPayable no Dynamics 365 Business central, que está mostrando o envelhecimento de uma conta de fornecedor.

## <a name="methods"></a>Métodos

| Método         | Tipo de retorno  |Descrição|
|:---------------|:-------------|:----------|
|[Obter agedAccountsPayable](../api/dynamics-agedaccountspayable-get.md)|agedAccountsPayable|Obter o objeto agedAccountsPayable|

## <a name="properties"></a>Propriedades
| Propriedade      | Tipo     |Descrição                                 |
|:--------------|:---------|:-------------------------------------------|
|VendorID       |GUID      |A ID exclusiva do fornecedor.                    |
|vendorNumber   |string    |Especifica o número do fornecedor.                  |
|name           |string    |Especifica o nome do fornecedor.                    |
|currencyCode   |string    |Especifica a moeda.                     |
|balanceDue     |numéricos   |Especifica o saldo total devido ao fornecedor.|
|currentAmount  |numéricos   |Especifica o saldo antes do primeiro período de envelhecimento.|
|period1Amount  |numéricos   |Especifica o saldo no primeiro período de classificação por vencimento.|
|period2Amount  |numéricos   |Especifica o saldo no segundo período de envelhecimento.|
|period3Amount  |numéricos   |Especifica o saldo no terceiro período de envelhecimento.|
|agedAsOfDate   |data|Especifica a data de início do período usada para calcular os períodos de expiração.|
|periodLengthFilter|string |Especifica o comprimento dos períodos. Os valores aceitáveis para as unidades de tempo são: D, WD, W, M, Q ou Y. C, o que significa unidade de tempo atual com base na data, pode ser especificado como um prefixo para a unidade de tempo.|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


```json
{
    "vendorId": "GUID",
    "vendorNumber": "string",
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
