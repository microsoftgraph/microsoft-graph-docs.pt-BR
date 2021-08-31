---
title: Tipo de recurso macOSAppleEventReceiver
description: Representa um processo que pode receber uma notificação de evento da Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 14f68bfa31c41b96e2a2dd160fa732d2c38e9b2f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58810644"
---
# <a name="macosappleeventreceiver-resource-type"></a>Tipo de recurso macOSAppleEventReceiver

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um processo que pode receber uma notificação de evento da Apple.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|codeRequirement|Cadeia de caracteres|Requisito de código para o aplicativo ou binário que recebe o Evento Apple.|
|identificador|Cadeia de caracteres|ID do pacote do aplicativo ou caminho do arquivo do processo ou executável que recebe o Evento Apple.|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|Use a ID do pacote para um aplicativo ou caminho para um processo ou executável que recebe o Evento Apple. Os valores possíveis são: `bundleID` e `path`.|
|allowed|Boleano|Permitir ou impedir que esse aplicativo receba eventos da Apple.|

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



