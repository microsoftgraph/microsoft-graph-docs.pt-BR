---
title: tipo de recurso macOSKernelExtension
description: Representa uma extensão de kernel macOS específica. Uma extensão de kernel macOS pode ser descrita por seu identificador de equipe e seu identificador de pacote.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fbf12bd16bdf606010bc9b6518c8241fe28eb765
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321929"
---
# <a name="macoskernelextension-resource-type"></a>tipo de recurso macOSKernelExtension

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa uma extensão de kernel macOS específica. Uma extensão de kernel macOS pode ser descrita por seu identificador de equipe e seu identificador de pacote.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|teamIdentifier|String|O identificador de equipe que foi usado para assinar a extensão do kernel.|
|bundleId|String|ID do pacote da extensão do kernel.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKernelExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKernelExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```



