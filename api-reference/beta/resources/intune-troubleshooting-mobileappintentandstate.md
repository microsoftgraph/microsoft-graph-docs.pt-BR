---
title: Tipo de recurso mobileAppIntentAndState
description: Estado de instalação e intenção do MobileApp para um determinado dispositivo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 40d555aacab29757622bb6e82d5358eb0c89ed42
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023259"
---
# <a name="mobileappintentandstate-resource-type"></a>Tipo de recurso mobileAppIntentAndState

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de instalação e intenção do MobileApp para um determinado dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppIntentAndStates](../api/intune-troubleshooting-mobileappintentandstate-list.md)|[Coleção mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Listar propriedades e relações dos [objetos mobileAppIntentAndState.](../resources/intune-troubleshooting-mobileappintentandstate.md)|
|[Obter mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Ler propriedades e relações do [objeto mobileAppIntentAndState.](../resources/intune-troubleshooting-mobileappintentandstate.md)|
|[Criar mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Crie um novo [objeto mobileAppIntentAndState.](../resources/intune-troubleshooting-mobileappintentandstate.md)|
|[Excluir mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|Nenhum|Exclui um [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).|
|[Atualizar mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Atualize as propriedades de [um objeto mobileAppIntentAndState.](../resources/intune-troubleshooting-mobileappintentandstate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O UUID do objeto.|
|managedDeviceIdentifier|Cadeia de caracteres|Identificador de dispositivo criado ou coletado pelo Intune.|
|userId|Cadeia de caracteres|Identificador do usuário que tentou registrar o dispositivo.|
|mobileAppList|[Coleção mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)|A lista de intenções de carga e estados para o locatário.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppIntentAndState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "String (identifier)",
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "String",
      "displayName": "String",
      "mobileAppIntent": "String",
      "displayVersion": "String",
      "installState": "String",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "String",
          "minimumOperatingSystemVersion": "String",
          "maximumOperatingSystemVersion": "String"
        }
      ]
    }
  ]
}
```




