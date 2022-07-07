---
title: Tipo de recurso remoteAssistanceReporting
description: Os recursos RemoteAssistanceReporting representam os metadados de uma determinada carga de relatório de Assistência Remota
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 65ca73ed17e70e9d4a86439a1daea490b84b30bc
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668647"
---
# <a name="remoteassistancereporting-resource-type"></a>Tipo de recurso remoteAssistanceReporting

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Os recursos RemoteAssistanceReporting representam os metadados de uma determinada carga de relatório de Assistência Remota

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo para uma sessão e para a carga de relatório de cada sessão|
|startDateTime|DateTimeOffset|Hora de início da sessão|
|endDateTime|DateTimeOffset|Hora de término da sessão|
|remoteAssistanceSessionType|[remoteAssistanceSessionType](../resources/intune-remoteassistance-remoteassistancesessiontype.md)|Tipo da sessão de assistência remota que foi mantida. Os valores possíveis são: `viewOnly`, `fullControl`, `elevation`. Os valores possíveis são: `viewOnly`, `fullControl`, `elevation`.|
|helperEmail|Cadeia de caracteres|Email de logon usado pelo auxiliar para estabelecer a sessão|
|helperTenantId|Cadeia de caracteres|ID do locatário para o auxiliar|
|helperFirstName|Cadeia de caracteres|Nome do auxiliar|
|helperLastName|Cadeia de caracteres|Sobrenome do auxiliar|
|auxiliares|Cadeia de caracteres|Sistema operacional do auxiliar|
|helperDeviceAadId|Cadeia de caracteres|ID do AAD do dispositivo auxiliar|
|helperDeviceName|Cadeia de caracteres|Nome do dispositivo do auxiliar|
|helperEnrollmentState|[enrollmentState](../resources/intune-remoteassistance-enrollmentstate.md)|Intune estado de registro do dispositivo do auxiliar. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|sharerEmail|String|Email de logon usado pelo sharer para estabelecer a sessão|
|sharerTenantId|Cadeia de caracteres|ID do locatário para o compartilhamento|
|sharerFirstName|Cadeia de caracteres|Nome do Sharer|
|sharerLastName|Cadeia de caracteres|Sobrenome do Sharer|
|sharerDeviceAadId|Cadeia de caracteres|ID do AAD do dispositivo do Sharer|
|sharerDeviceName|String|Nome do dispositivo do Sharer|
|sharerOs|Cadeia de caracteres|Sistema operacional do Sharer|
|sharerEnrollmentState|[enrollmentState](../resources/intune-remoteassistance-enrollmentstate.md)|Intune estado de registro do dispositivo do sharer. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteAssistanceReporting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistanceReporting",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "remoteAssistanceSessionType": "String",
  "helperEmail": "String",
  "helperTenantId": "String",
  "helperFirstName": "String",
  "helperLastName": "String",
  "helperOs": "String",
  "helperDeviceAadId": "String",
  "helperDeviceName": "String",
  "helperEnrollmentState": "String",
  "sharerEmail": "String",
  "sharerTenantId": "String",
  "sharerFirstName": "String",
  "sharerLastName": "String",
  "sharerDeviceAadId": "String",
  "sharerDeviceName": "String",
  "sharerOs": "String",
  "sharerEnrollmentState": "String"
}
```




