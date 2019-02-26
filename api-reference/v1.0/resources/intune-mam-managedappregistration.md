---
title: Tipo de recurso managedAppRegistration
description: O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos. O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc4754a190f19dab34ac417d2852ccc9e06ba9f4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252235"
---
# <a name="managedappregistration-resource-type"></a>Tipo de recurso managedAppRegistration

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.
O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.

## <a name="methods"></a>Métodos
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
|applicationVersion|String|Versão do Aplicativo|
|managementSdkVersion|String|Versão do SDK de gerenciamento do aplicativo|
|platformVersion|String|Versão do sistema operacional|
|deviceType|String|Tipo de dispositivo do host|
|deviceTag|Cadeia de caracteres|Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo. Sem garantia de indicar aplicativos em todas as condições.|
|deviceName|Cadeia de caracteres|Nome do dispositivo do host|
|flaggedReasons|coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)|Zero ou mais motivos para a sinalização de um registro de aplicativo. E.g. aplicativo usado em dispositivo modificado|
|userId|String|A ID de usuário à qual este registro de aplicativo pertence.|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|O identificador do pacote do aplicativo|
|id|String|Chave da entidade.|
|version|String|Versão da entidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appliedPolicies|Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.|
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
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-managedappregistration.md/microsoft.graph.managedAppRegistration/flaggedReasons:
    Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->


