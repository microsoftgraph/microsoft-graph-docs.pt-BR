---
title: tipo de recurso paymentTerms
description: Um objeto de condições de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4ed1f3791474cf6e29038e75fcd3625e4da300a0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365637"
---
# <a name="paymentterms-resource-type"></a>tipo de recurso paymentTerms
Representa um termo de pagamento no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método                                                      | Tipo de retorno|Descrição            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[Obter paymentTerms](../api/dynamics-paymentterms-get.md)      |paymentTerms|Obter um objeto de condições de pagamento.   |
|[Postar paymentTerms](../api/dynamics-create-paymentterms.md)  |paymentTerms|Criar um objeto de condições de pagamento.|
|[Patch paymentTerms](../api/dynamics-paymentterms-update.md) |paymentTerms|Atualizar um objeto de condições de pagamento.|
|[Excluir paymentTerms](../api/dynamics-paymentterms-delete.md)|Nenhuma        |Excluir um objeto de condições de pagamento.|

## <a name="properties"></a>Propriedades
| Propriedade                     | Tipo     |Descrição                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|id                            |GUID    |A ID exclusiva do paymentTerms. Não editável.           |
|código                          |string  |Especifica o código da expressão de pagamento.                           |
|displayName                   |string  |Especifica o nome de exibição do termo de pagamento.                   |
|dueDateCalculation            |string  |Especifica a fórmula usada para calcular a data em que um pagamento deve ser feito.|
|discountDateCalculation       |string  |Especifica a fórmula usada para calcular a data em que um pagamento deve ser feito para obter um desconto.|
|discountPercent               |dígitos |Especifica a porcentagem de desconto aplicada ao pagamento antecipado de um valor de fatura.|
|calculateDiscountOnCreditMemos|boolean |Especifica se o desconto deve ser aplicado a memorandos de crédito. **True** indica que um desconto será fornecido, **false** indica que um desconto não será fornecido.|
|lastModifiedDateTime          |DateTime|O último DateTime que o paymentTerms foi modificado. Somente Leitura.|  


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do paymentTerms.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "dueDateCalculation": "string",
  "discountDateCalculation": "string",
  "discountPercent": "decimal",
  "calculateDiscountOnCreditMemos": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
