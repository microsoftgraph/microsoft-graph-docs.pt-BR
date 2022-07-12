---
title: Tipo de recurso deviceAppManagement
description: Entidade singleton de gerenciamento de aplicativos do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a2a982b98a4c1d8c56d7069afacd74ad8c46c67f
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730613"
---
# <a name="deviceappmanagement-resource-type"></a>Tipo de recurso deviceAppManagement

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade singleton de gerenciamento de aplicativos do dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedAppPolicies|Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Políticas de aplicativos gerenciados.|
|iosManagedAppProtections|Coleção [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)|Políticas de aplicativos gerenciados para iOS.|
|androidManagedAppProtections|Coleção [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md)|Políticas de aplicativos gerenciados para Android.|
|defaultManagedAppProtections|Coleção [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Políticas de aplicativos gerenciados padrão.|
|targetedManagedAppConfigurations|Coleção [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)|Configurações de aplicativos gerenciados direcionadas.|
|mdmWindowsInformationProtectionPolicies|Coleção [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|Proteção de informações do Windows para aplicativos em execução em dispositivos que estão registrados no MDM.|
|windowsInformationProtectionPolicies|Coleção [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)|Proteção de informações do Windows para aplicativos em execução em dispositivos que não estão registrados no MDM.|
|managedAppRegistrations|Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Os registros de aplicativos gerenciados.|
|managedAppStatuses|Coleção [managedAppStatus](../resources/intune-mam-managedappstatus.md)|Os status de aplicativos gerenciados.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```





