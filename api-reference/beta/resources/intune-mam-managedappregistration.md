---
title: Tipo de recurso managedAppRegistration
description: O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos. O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2d527b4d0a6da5a54a6e167db063b8c4e06a6062
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444179"
---
# <a name="managedappregistration-resource-type"></a>Tipo de recurso managedAppRegistration

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.
O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAppRegistrations](../api/intune-mam-managedappregistration-list.md)|Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Listar propriedades e relações dos objetos de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|[Obter managedAppRegistrations](../api/intune-mam-managedappregistration-get.md)|[managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Ler propriedades e relações do objeto [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|[função getUserIdsWithFlaggedAppRegistration](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|Coleção String|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Data e hora de criação|
|lastSyncDateTime|DateTimeOffset|Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.|
|applicationVersion|Cadeia de caracteres|Versão do Aplicativo|
|managementSdkVersion|Cadeia de caracteres|Versão do SDK de gerenciamento do aplicativo|
|platformVersion|Cadeia de caracteres|Versão do sistema operacional|
|deviceType|Cadeia de caracteres|Tipo de dispositivo do host|
|deviceTag|String|Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo. Sem garantia de indicar aplicativos em todas as condições.|
|deviceName|Cadeia de caracteres|Nome do dispositivo do host|
|managedDeviceId|String|O identificador de Dispositivo Gerenciado do dispositivo host. O valor pode estar vazio mesmo quando o dispositivo host é gerenciado.|
|azureADDeviceId|String|O identificador do Dispositivo do Azure Active Directory do dispositivo host. O valor pode estar vazio mesmo quando o dispositivo host é registrado no Azure Active Directory.|
|deviceModel|Cadeia de caracteres|O modelo de dispositivo para o registro do aplicativo atual |
|deviceManufacturer|String|O fabricante do dispositivo para o registro do aplicativo atual |
|flaggedReasons|[Coleção managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)|Zero ou mais motivos para a sinalização de um registro de aplicativo. E.g. aplicativo usado em dispositivo modificado|
|userId|Cadeia de caracteres|A ID de usuário à qual este registro de aplicativo pertence.|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|O identificador do pacote do aplicativo|
|id|String|Chave da entidade.|
|versão|String|Versão da entidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appliedPolicies|Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Zero ou mais políticas já aplicadas no aplicativo registrado quando ele foi sincronizado pela última vez com o serviço de gerenciamento.|
|intendedPolicies|Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.|
|operations|Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)|Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
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
    "@odata.type": "microsoft.graph.windowsAppIdentifier",
    "windowsAppId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




