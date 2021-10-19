---
title: Tipo de recurso remoteAssistanceReporting
description: Recursos RemoteAssistanceReporting representam os metadados de uma determinada carga de relatórios de Assistência Remota
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 65103b951d41328d4e1b414a06ef99b8a99001bd
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60485160"
---
# <a name="remoteassistancereporting-resource-type"></a>Tipo de recurso remoteAssistanceReporting

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Recursos RemoteAssistanceReporting representam os metadados de uma determinada carga de relatórios de Assistência Remota

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo para uma sessão e para a carga de relatórios de cada sessão|
|startDateTime|DateTimeOffset|Hora de início da sessão|
|endDateTime|DateTimeOffset|Hora de término da sessão|
|remoteAssistanceSessionType|[remoteAssistanceSessionType](../resources/intune-remoteassistance-remoteassistancesessiontype.md)|Tipo da sessão de assistência remota realizada. Os valores possíveis são: `viewOnly`, `fullControl`, `elevation`. Os valores possíveis são: `viewOnly`, `fullControl`, `elevation`.|
|helperEmail|Cadeia de caracteres|Logon de email usado pelo auxiliar para estabelecer a sessão|
|helperTenantId|Cadeia de caracteres|ID do locatário para o auxiliar|
|helperFirstName|Cadeia de caracteres|Nome do auxiliar|
|helperLastName|Cadeia de caracteres|Sobrenome do auxiliar|
|helperOs|Cadeia de caracteres|Sistema operacional do auxiliar|
|helperDeviceAadId|Cadeia de caracteres|O dispositivo do auxiliar AAD ID|
|helperDeviceName|Cadeia de caracteres|Nome do dispositivo do auxiliar|
|helperEnrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Estado de registro do intune do dispositivo do auxiliar. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|sharerEmail|Cadeia de caracteres|Logon de email usado pelo sharer para estabelecer a sessão|
|sharerTenantId|Cadeia de caracteres|ID de locatário para o sharer|
|sharerFirstName|Cadeia de caracteres|Nome do Sharer|
|sharerLastName|Cadeia de caracteres|Sobrenome do Sharer|
|sharerDeviceAadId|Cadeia de caracteres|O dispositivo do Sharer AAD ID|
|sharerDeviceName|Cadeia de caracteres|Nome do dispositivo do Sharer|
|sharerOs|Cadeia de caracteres|Sistema operacional do Sharer|
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



