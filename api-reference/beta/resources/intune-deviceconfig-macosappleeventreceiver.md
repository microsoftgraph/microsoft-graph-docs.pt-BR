---
title: tipo de recurso macOSAppleEventReceiver
description: Representa um processo que pode receber uma notificação de evento Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db781ad536e8fe918257f74d87fa104f4b2a23f1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055446"
---
# <a name="macosappleeventreceiver-resource-type"></a>tipo de recurso macOSAppleEventReceiver

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um processo que pode receber uma notificação de evento Apple.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|codeRequirement|Cadeia de caracteres|Requisito de código para o aplicativo ou o binário que recebe o evento Apple.|
|identificador|Cadeia de caracteres|ID de pacote do aplicativo ou caminho de arquivo do processo ou executável que recebe o evento Apple.|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|Use ID de pacote para um aplicativo ou caminho para um processo ou executável que receba o evento Apple. Os valores possíveis são: `bundleID` e `path`.|
|autorizado|Booliano|Permitir ou impedir que este aplicativo receba eventos Apple.|

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






