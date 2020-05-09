---
title: tipo de recurso macOSAppleEventReceiver
description: Representa um processo que pode receber uma notificação de evento Apple.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 16064b1f7311f8ab384d7905a6f4cfa2f09ccc09
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177349"
---
# <a name="macosappleeventreceiver-resource-type"></a>tipo de recurso macOSAppleEventReceiver

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um processo que pode receber uma notificação de evento Apple.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|codeRequirement|Cadeia de Caracteres|Requisito de código para o aplicativo ou o binário que recebe o evento Apple.|
|identificador|Cadeia de Caracteres|ID de pacote do aplicativo ou caminho de arquivo do processo ou executável que recebe o evento Apple.|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|Use ID de pacote para um aplicativo ou caminho para um processo ou executável que receba o evento Apple. Os valores possíveis são: `bundleID` e `path`.|
|autorizado|Boolean|Permitir ou impedir que este aplicativo receba eventos Apple.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAppleEventReceiver"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAppleEventReceiver",
  "codeRequirement": "String",
  "identifier": "String",
  "identifierType": "String",
  "allowed": true
}
```



