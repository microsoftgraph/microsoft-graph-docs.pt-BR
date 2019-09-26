---
title: Tipo de recurso deviceEnrollmentConfiguration
description: A classe base da configuração de registro do dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 79941f498efae8167e6d9abcd9bcdf78b9557677
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199615"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a>Tipo de recurso deviceEnrollmentConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A classe base da configuração de registro do dispositivo

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceEnrollmentConfigurations](../api/intune-shared-deviceenrollmentconfiguration-list.md)|Conjunto [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|Listar propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).|
|[Obter deviceEnrollmentConfiguration](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|Ler propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).|
|**Integração**|
|[Ação setPriority](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|Nenhum|Ainda não documentado|
|[atribuir ação](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|Nenhuma|Ainda não documentado|
|**Conjunto de políticas**|
|[ação hasPayloadLinks](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para a conta|
|displayName|String|O nome de exibição da configuração de registro do dispositivo|
|descrição|String|A descrição da configuração de registro do dispositivo|
|prioridade|Int32|A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro. Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.|
|createdDateTime|DateTimeOffset|Data e hora de criação em UTC da configuração de registro do dispositivo|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação em UTC da configuração de registro do dispositivo|
|versão|Int32|A versão da configuração de registro do dispositivo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Integração**|
|atribuições|Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024
}
```



