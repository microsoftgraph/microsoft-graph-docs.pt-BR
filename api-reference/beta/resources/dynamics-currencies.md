---
title: tipo de recurso moedas
description: Um objeto Currency no Dynamics 365 Business central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: e986777d277e84246104561e5e275d7508b41b7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504731"
---
# <a name="currencies-resource-type"></a>tipo de recurso moedas

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma moeda usada no Dynamics 365 Business central.

## <a name="methods"></a>Métodos
| Método                                                  |Tipo de retorno|Descrição       |
|:--------------------------------------------------------|:----------|:-----------------|
|[Obter moedas](../api/dynamics-currencies-get.md)      |monetária |Obter uma moeda.   |
|[Lançar moedas](../api/dynamics-create-currencies.md)  |monetária |Criar uma moeda.|
|[Corrigir moedas](../api/dynamics-currencies-update.md) |monetária |Atualize uma moeda.|
|[Excluir moedas](../api/dynamics-currencies-delete.md)|nenhuma       |Excluir uma moeda.|

## <a name="properties"></a>Propriedades
| Propriedade              | Tipo   |Descrição                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|id                     |GUID    |A identificação exclusiva da moeda. Não editável.                  |
|código                   |cadeia de caracteres  |Especifica o código da moeda.                                  |
|displayName            |string  |Especifica o nome de exibição da moeda.                          |
|formato                 |string  |Especifica o símbolo para esta moeda que aparece nos cheques.|
|amountDecimalPlaces    |string  |Especifica o número de casas decimais que o sistema exibirá em valores dessa moeda.|
|amountRoundingPrecision|dígitos |Especifica o tamanho do intervalo a ser usado ao arredondar valores para esta moeda.|
|lastModifiedDateTime   |datetime|O último DateTime que a moeda foi modificada. Somente leitura.       |  


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

