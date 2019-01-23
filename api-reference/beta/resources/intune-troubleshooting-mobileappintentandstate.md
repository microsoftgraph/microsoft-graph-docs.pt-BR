---
title: tipo de recurso de mobileAppIntentAndState
description: A intenção de MobileApp e estado de instalação para um determinado dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 01792d30bdf821d4dd0795926e116bdc12b95ad9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402402"
---
# <a name="mobileappintentandstate-resource-type"></a>tipo de recurso de mobileAppIntentAndState

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

A intenção de MobileApp e estado de instalação para um determinado dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista mobileAppIntentAndStates](../api/intune-troubleshooting-mobileappintentandstate-list.md)|coleção [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Lista as propriedades e os relacionamentos dos objetos [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .|
|[Obter mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Leia as propriedades e os relacionamentos do objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .|
|[Criar mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Crie um novo objeto de [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .|
|[Excluir mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|Nenhum|Exclui um [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).|
|[Atualizar mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Atualize as propriedades de um objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O UUID do objeto.|
|managedDeviceIdentifier|Cadeia de caracteres|Identificador de dispositivo criado ou coletado pelo Intune.|
|userId|Cadeia de caracteres|Identificador do usuário que tentou registrar o dispositivo.|
|mobileAppList|coleção [mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)|A lista de propósitos de carga e estados do inquilino.|

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




