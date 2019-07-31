---
title: tipo de recurso moedas
description: Um objeto Currency no Dynamics 365 Business central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ba8ad750831394e2a84fab7ca87d76754838db60
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012615"
---
# <a name="currencies-resource-type"></a>tipo de recurso moedas
Representa uma moeda usada no Dynamics 365 Business central.

## <a name="methods"></a>Métodos
| Método                                                  |Tipo de retorno|Descrição       |
|:--------------------------------------------------------|:----------|:-----------------|
|[Obter moedas](../api/dynamics-currencies-get.md)      |monetária |Obter uma moeda.   |
|[Lançar moedas](../api/dynamics-create-currencies.md)  |monetária |Criar uma moeda.|
|[Corrigir moedas](../api/dynamics-currencies-update.md) |monetária |Atualize uma moeda.|
|[Excluir moedas](../api/dynamics-currencies-delete.md)|none       |Excluir uma moeda.|

## <a name="properties"></a>Propriedades
| Propriedade              | Tipo   |Descrição                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|id                     |GUID    |A identificação exclusiva da moeda. Não editável.                  |
|código                   |cadeia de caracteres  |Especifica o código da moeda.                                  |
|displayName            |string  |Especifica o nome de exibição da moeda.                          |
|formato                 |string  |Especifica o símbolo para esta moeda que aparece nos cheques.|
|amountDecimalPlaces    |string  |Especifica o número de casas decimais que o sistema exibirá em valores dessa moeda.|
|amountRoundingPrecision|dígitos |Especifica o tamanho do intervalo a ser usado ao arredondar valores para esta moeda.|
|lastModifiedDateTime   |DateTime|O último DateTime que a moeda foi modificada. Somente leitura.       |  


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

