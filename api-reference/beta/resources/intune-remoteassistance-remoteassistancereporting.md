---
title: Tipo de recurso remoteAssistanceReporting
description: Recursos RemoteAssistanceReporting representam os metadados de uma determinada carga de relatórios de Assistência Remota
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a2fb437a3b6b2cb44f32cc1e12a601b3ed4673ac
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61338138"
---
# <a name="remoteassistancereporting-resource-type"></a>Tipo de recurso remoteAssistanceReporting

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Recursos RemoteAssistanceReporting representam os metadados de uma determinada carga de relatórios de Assistência Remota

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo para uma sessão e para a carga de relatórios de cada sessão|
|startDateTime|DateTimeOffset|Hora de início da sessão|
|endDateTime|DateTimeOffset|Hora de término da sessão|
|remoteAssistanceSessionType|[remoteAssistanceSessionType](../resources/intune-remoteassistance-remoteassistancesessiontype.md)|Tipo da sessão de assistência remota realizada. Os valores possíveis são: `viewOnly`, `fullControl`, `elevation`. Os valores possíveis são: `viewOnly`, `fullControl`, `elevation`.|
|helperEmail|String|Logon de email usado pelo auxiliar para estabelecer a sessão|
|helperTenantId|String|ID do locatário para o auxiliar|
|helperFirstName|String|Nome do auxiliar|
|helperLastName|String|Sobrenome do auxiliar|
|helperOs|String|Sistema operacional do auxiliar|
|helperDeviceAadId|String|O dispositivo do auxiliar AAD ID|
|helperDeviceName|String|Nome do dispositivo do auxiliar|
|helperEnrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Estado de registro do intune do dispositivo do auxiliar. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|sharerEmail|String|Logon de email usado pelo sharer para estabelecer a sessão|
|sharerTenantId|String|ID de locatário para o sharer|
|sharerFirstName|String|Nome do Sharer|
|sharerLastName|String|Sobrenome do Sharer|
|sharerDeviceAadId|String|O dispositivo do Sharer AAD ID|
|sharerDeviceName|String|Nome do dispositivo do Sharer|
|sharerOs|String|Sistema operacional do Sharer|
|sharerEnrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Estado de registro do intune do dispositivo do sharer. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|

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




