---
title: iosManagedAppRegistration resource type
description: Representa os detalhes de sincronização de um aplicativo para iOS, com recursos de gerenciamento, para um usuário específico.
localization_priority: Normal
ms.openlocfilehash: eb36bf1e96a8b7a54daf9d02b4cc2765a1844d4c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868065"
---
# <a name="iosmanagedappregistration-resource-type"></a>iosManagedAppRegistration resource type

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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
|applicationVersion|Cadeia de caracteres|Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|managementSdkVersion|Cadeia de caracteres|Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|platformVersion|Cadeia de caracteres|Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceType|Cadeia de caracteres|Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceTag|Cadeia de caracteres|Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo. Sem garantia de indicar aplicativos em todas as condições. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceName|Cadeia de caracteres|Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|flaggedReasons|coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)|Zero ou mais motivos para a sinalização de um registro de aplicativo. E.g. Aplicativo em execução em um dispositivo root. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|userId|Cadeia de caracteres|A ID de usuário à qual este registro de aplicativo pertence. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|version|Cadeia de caracteres|Versão da entidade. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|

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
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier",
    "bundleId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-iosmanagedappregistration.md/microsoft.graph.iosManagedAppRegistration/flaggedReasons:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->
