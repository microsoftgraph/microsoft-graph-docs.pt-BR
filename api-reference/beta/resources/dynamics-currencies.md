---
title: tipo de recurso de moedas
description: Um objeto currency no Dynamics 365 Business Central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.localizationpriority: medium
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 228f4c227cd8c0efa5f2ed6dcd885c81a2f5f9ab
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767080"
---
# <a name="currencies-resource-type"></a>tipo de recurso de moedas

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma moeda usada no Dynamics 365 Business Central.

## <a name="methods"></a>Métodos
| Método                                                  |Tipo de retorno|Descrição       |
|:--------------------------------------------------------|:----------|:-----------------|
|[Obter moedas](../api/dynamics-currencies-get.md)      |moedas |Obter uma Conversor de Moedas.   |
|[Post currencies](../api/dynamics-create-currencies.md)  |moedas |Crie uma Conversor de Moedas.|
|[Patch currencies](../api/dynamics-currencies-update.md) |moedas |Atualize um Conversor de Moedas.|
|[Excluir moedas](../api/dynamics-currencies-delete.md)|none       |Exclua um Conversor de Moedas.|

## <a name="properties"></a>Propriedades
| Propriedade              | Tipo   |Descrição                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|id                     |GUID    |A ID exclusiva da moeda. Não editável.                  |
|código                   |cadeia de caracteres  |Especifica o código de moeda.                                  |
|displayName            |string  |Especifica o nome de exibição de moeda.                          |
|symbol                 |string  |Especifica o símbolo dessa moeda que aparece em verificações.|
|amountDecimalPlaces    |string  |Especifica o número de casas decimais que o sistema exibirá em valores para essa moeda.|
|amountRoundingPrecision|decimal |Especifica o tamanho do intervalo a ser usado ao arredondamento de valores para essa moeda.|
|lastModifiedDateTime   |datetime|A última data em que a moeda foi modificada. Somente leitura.       |  


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON das moedas.


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



