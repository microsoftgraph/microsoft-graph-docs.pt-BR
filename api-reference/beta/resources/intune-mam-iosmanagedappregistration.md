---
title: iosManagedAppRegistration resource type
description: Representa os detalhes de sincronização de um aplicativo para iOS, com recursos de gerenciamento, para um usuário específico. O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: baf8d9b845781a17cf0188bdae6f31d3601265b9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415744"
---
# <a name="iosmanagedappregistration-resource-type"></a>iosManagedAppRegistration resource type

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Representa os detalhes de sincronização de um aplicativo para iOS, com recursos de gerenciamento, para um usuário específico.
O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.


Herda de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosManagedAppRegistrations](../api/intune-mam-iosmanagedappregistration-list.md)|Coleção [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md)|Lista propriedades e relações dos objetos [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).|
|[Obter iosManagedAppRegistration](../api/intune-mam-iosmanagedappregistration-get.md)|[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md)|Ler propriedades e relações do objeto [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Data e hora de criação. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|lastSyncDateTime|DateTimeOffset|Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|applicationVersion|String|Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|managementSdkVersion|String|Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|platformVersion|String|Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceType|String|Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceTag|String|Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo. Sem garantia de indicar aplicativos em todas as condições. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceName|String|Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|managedDeviceId|String|O identificador de dispositivo gerenciado do dispositivo de host. Valor poderia ser vazia, mesmo quando o dispositivo do host é gerenciado. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|azureADDeviceId|String|O identificador de dispositivo do Azure Active Directory do dispositivo de host. Valor poderia ser vazia, mesmo quando o dispositivo do host é o Azure Active Directory registrada. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceModel|Cadeia de caracteres|O modelo de dispositivo para que o registro atual do aplicativo Inherited de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceManufacturer|String|O fabricante do dispositivo para que o registro atual do aplicativo Inherited de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|flaggedReasons|coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)|Zero ou mais motivos para a sinalização de um registro de aplicativo. E.g. Aplicativo em execução em um dispositivo root. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|userId|String|A ID de usuário à qual este registro de aplicativo pertence. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|id|String|Chave da entidade. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|version|String|Versão da entidade. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appliedPolicies|Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|intendedPolicies|Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|operations|Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)|Zero ou mais operações de longa execução desencadeadas no registro do aplicativo. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosManagedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "managedDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
    "bundleId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




