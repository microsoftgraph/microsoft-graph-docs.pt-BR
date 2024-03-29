---
title: Tipo de recurso macOSKernelExtension
description: Representa uma extensão de kernel do macOS específica. Uma extensão de kernel macOS pode ser descrita pelo identificador de equipe, além do identificador de pacote.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8f430f83dbd166ee93f9e0ebfc4baa4ddb9f39db
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095567"
---
# <a name="macoskernelextension-resource-type"></a>Tipo de recurso macOSKernelExtension

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa uma extensão de kernel do macOS específica. Uma extensão de kernel macOS pode ser descrita pelo identificador de equipe, além do identificador de pacote.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|teamIdentifier|Cadeia de Caracteres|O identificador de equipe usado para assinar a extensão do kernel.|
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



