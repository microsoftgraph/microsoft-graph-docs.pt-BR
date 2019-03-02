---
title: tipo de recurso moedas
description: Um objeto Currency no Dynamics 365 Business central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: c0d15b8d20e99537cb2f567a9f8fe12b45dbd389
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366624"
---
# <a name="currencies-resource-type"></a>tipo de recurso moedas
Representa uma moeda usada no Dynamics 365 Business central.

## <a name="methods"></a>Métodos
| Método                                                  |Tipo de retorno|Descrição       |
|:--------------------------------------------------------|:----------|:-----------------|
|[Obter moedas](../api/dynamics-currencies-get.md)      |monetária |Obter uma moeda.   |
|[Lançar moedas](../api/dynamics-create-currencies.md)  |monetária |Criar uma moeda.|
|[Corrigir moedas](../api/dynamics-currencies-update.md) |monetária |Atualize uma moeda.|
|[Excluir moedas](../api/dynamics-currencies-delete.md)|Nenhuma       |Excluir uma moeda.|

## <a name="properties"></a>Propriedades
| Propriedade              | Tipo   |Descrição                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|id                     |GUID    |A identificação exclusiva da moeda. Não editável.                  |
|código                   |string  |Especifica o código da moeda.                                  |
|displayName            |string  |Especifica o nome de exibição da moeda.                          |
|formato                 |string  |Especifica o símbolo para esta moeda que aparece nos cheques.|
|amountDecimalPlaces    |string  |Especifica o número de casas decimais que o sistema exibirá em valores dessa moeda.|
|amountRoundingPrecision|dígitos |Especifica o tamanho do intervalo a ser usado ao arredondar valores para esta moeda.|
|lastModifiedDateTime   |DateTime|O último DateTime que a moeda foi modificada. Somente Leitura.       |  


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON das moedas.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "symbol": "string",
  "amountDecimalPlaces": "string",
  "amountRoundingPrecision": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

