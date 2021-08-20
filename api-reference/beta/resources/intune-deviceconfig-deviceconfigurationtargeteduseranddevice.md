---
title: Tipo de recurso deviceConfigurationTargetedUserAndDevice
description: Resumo de conflitos para um conjunto de políticas de configuração de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 671cbd9e5c6cf9448b86f8ce3f1bd852b794ca492e55b9c0edcbde8a01e0a3c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227474"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>Tipo de recurso deviceConfigurationTargetedUserAndDevice

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Resumo de conflitos para um conjunto de políticas de configuração de dispositivo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceId|Cadeia de caracteres|A id do dispositivo na verificação.|
|deviceName|String|O nome do dispositivo no check-in.|
|userId|Cadeia de caracteres|A id do usuário no check-in.|
|userDisplayName|Cadeia de caracteres|O nome de exibição do usuário na verificação|
|userPrincipalName|Cadeia de caracteres|O UPN do usuário no check-in.|
|lastCheckinDateTime|DateTimeOffset|Última verificação em tempo para esse par de usuários/dispositivos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationTargetedUserAndDevice",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```




