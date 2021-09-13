---
title: Tipo de recurso remoteAssistanceReporting
description: Recursos RemoteAssistanceReporting representam os metadados de uma determinada carga de relatórios de Assistência Remota
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7793b8ef8bffa33e5d2e77de9fd102b9d0c59288
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039459"
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
|helperEmail|Cadeia de Caracteres|Logon de email usado pelo auxiliar para estabelecer a sessão|
|helperTenantId|Cadeia de Caracteres|ID do locatário para o auxiliar|
|helperFirstName|Cadeia de Caracteres|Nome do auxiliar|
|helperLastName|Cadeia de Caracteres|Sobrenome do auxiliar|
|helperDeviceAadId|Cadeia de Caracteres|ID do AAD do dispositivo auxiliar|
|helperDeviceName|Cadeia de Caracteres|Nome do dispositivo do auxiliar|
|helperEnrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Estado de registro do intune do dispositivo do auxiliar. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|sharerEmail|Cadeia de Caracteres|Logon de email usado pelo sharer para estabelecer a sessão|
|sharerTenantId|Cadeia de Caracteres|ID de locatário para o sharer|
|sharerFirstName|Cadeia de Caracteres|Nome do Sharer|
|sharerLastName|Cadeia de Caracteres|Sobrenome do Sharer|
|sharerDeviceAadId|Cadeia de Caracteres|ID AAD do dispositivo do Sharer|
|sharerDeviceName|Cadeia de Caracteres|Nome do dispositivo do Sharer|
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



