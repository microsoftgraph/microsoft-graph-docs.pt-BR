---
title: Tipo de recurso connectionQuota
description: Representa a cota de conexão que contém informações calculadas sobre a utilização da cota de uma conexão externa.
author: josmoran
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 968d0154a1a0bbc5fe33bdcad1123c0944e854fb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316538"
---
# <a name="connectionquota-resource-type"></a>Tipo de recurso connectionQuota

Namespace: microsoft.graph.externalConnectors

Representa a [cota de](externalconnectors-externalconnection.md) conexão que contém informações calculadas sobre a utilização da cota de uma conexão externa. Ele retorna o número permitido de itens que você pode ingerir em uma conexão considerando os itens ingeridos para a conexão em relação à cota no nível do locatário para conectores do Microsoft Graph.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Obter connectionQuota](../api/externalconnectors-connectionquota-get.md) |[connectionQuota](../resources/externalconnectors-connectionquota.md)| Recupere as propriedades e as relações de uma **connectionQuota**. |

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| itemsRemaining | Int64 | Retorna o número mínimo em um intervalo que contém os seguintes dados: itens *restantes* na conexão e itens restantes *no nível do locatário*. A equação a seguir representa a fórmula usada para calcular o número mínimo: `min(max capacity in the connection – number of items in the connection, tenant quota – number of items indexed in all connections)`. Se a conexão não formonetizada (versão prévia do conector ou experiência de conteúdo de visualização), ela retornará o número de itens restantes na conexão. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.connectionQuota",
  "openType": false
}
-->

``` json
{
  "itemsRemaining": "Int64"
}
```
