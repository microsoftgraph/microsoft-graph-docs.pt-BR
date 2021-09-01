---
title: Tipo de recurso remoteAssistanceReporting
description: Recursos RemoteAssistanceReporting representam os metadados de uma determinada carga de relatórios de Assistência Remota
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d5442ce93f5e7697ed577835ddd437252396e67b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805323"
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
|helperDeviceAadId|Cadeia de caracteres|ID do AAD do dispositivo auxiliar|
|helperDeviceName|Cadeia de caracteres|Nome do dispositivo do auxiliar|
|helperEnrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Estado de registro do intune do dispositivo do auxiliar. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|sharerEmail|Cadeia de caracteres|Logon de email usado pelo sharer para estabelecer a sessão|
|sharerTenantId|Cadeia de caracteres|ID de locatário para o sharer|
|sharerFirstName|Cadeia de caracteres|Nome do Sharer|
|sharerLastName|Cadeia de caracteres|Sobrenome do Sharer|
|sharerDeviceAadId|Cadeia de caracteres|ID AAD do dispositivo do Sharer|
|sharerDeviceName|Cadeia de caracteres|Nome do dispositivo do Sharer|
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
  "helperDeviceAadId": "String",
  "helperDeviceName": "String",
  "helperEnrollmentState": "String",
  "sharerEmail": "String",
  "sharerTenantId": "String",
  "sharerFirstName": "String",
  "sharerLastName": "String",
  "sharerDeviceAadId": "String",
  "sharerDeviceName": "String",
  "sharerEnrollmentState": "String"
}
```



