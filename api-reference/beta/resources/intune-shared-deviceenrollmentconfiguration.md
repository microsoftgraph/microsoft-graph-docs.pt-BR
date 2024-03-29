---
title: Tipo de recurso deviceEnrollmentConfiguration
description: A classe base de configuração de registro de dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 66ae56fd0e4d1812977bafcf87d29dca7c55cece
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436551"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a>Tipo de recurso deviceEnrollmentConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A classe base de configuração de registro de dispositivo

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceEnrollmentConfigurations](../api/intune-shared-deviceenrollmentconfiguration-list.md)|Conjunto [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|Listar propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).|
|[Obter deviceEnrollmentConfiguration](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|Ler propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).|
|**Integração**|
|[Ação setPriority](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|Nenhum|Ainda não documentado|
|[atribuir ação](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|Nenhuma|Ainda não documentado|
|**Conjunto de Políticas**|
|[Ação hasPayloadLinks](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|[coleção hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador Exclusivo da conta|
|displayName|Cadeia de caracteres|O nome de exibição da configuração de registro do dispositivo|
|description|Cadeia de caracteres|A descrição da configuração de registro do dispositivo|
|prioridade|Int32|A prioridade é usada quando um usuário existe em vários grupos que recebem a configuração de registro. Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixa.|
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



