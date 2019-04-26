---
title: tipo de recurso mobileAppIntentAndState
description: MobileApp tentativa e estado de instalação para um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e90251338ad7e740b216452a52cc0fffcfc44565
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558150"
---
# <a name="mobileappintentandstate-resource-type"></a>tipo de recurso mobileAppIntentAndState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

MobileApp tentativa e estado de instalação para um determinado dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppIntentAndStates](../api/intune-troubleshooting-mobileappintentandstate-list.md)|coleção [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Listar Propriedades e relações dos objetos [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .|
|[Obter mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Leia as propriedades e as relações do objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .|
|[Criar mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Criar um novo objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .|
|[Excluir mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|Nenhum|Exclui [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).|
|[Atualizar mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Atualiza as propriedades de um objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O UUID do objeto.|
|managedDeviceIdentifier|Cadeia de caracteres|Identificador de dispositivo criado ou coletado pelo Intune.|
|userId|String|Identificador do usuário que tentou registrar o dispositivo.|
|mobileAppList|coleção [mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)|A lista de efeitos e Estados de carga para o locatário.|

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



