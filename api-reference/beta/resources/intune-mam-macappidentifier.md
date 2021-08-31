---
title: Tipo de recurso macAppIdentifier
description: O identificador de um aplicativo Mac.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb61e5c7cac991a9c8e479f4de85fd1fd8f2c7ba
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789239"
---
# <a name="macappidentifier-resource-type"></a>Tipo de recurso macAppIdentifier

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O identificador de um aplicativo Mac.


Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|bundleId|Cadeia de caracteres|O identificador de um aplicativo, conforme especificado na App Store.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macAppIdentifier",
  "bundleId": "String"
}
```



