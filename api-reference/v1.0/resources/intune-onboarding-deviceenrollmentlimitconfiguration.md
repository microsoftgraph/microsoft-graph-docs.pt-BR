---
title: Tipo de recurso deviceEnrollmentLimitConfiguration
description: Configuração de Registro de Dispositivo que restringe o número de dispositivos que um usuário pode registrar
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 45daf117984f312c86dacd52cf1f1d06e5a7a4df
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730347"
---
# <a name="deviceenrollmentlimitconfiguration-resource-type"></a>Tipo de recurso deviceEnrollmentLimitConfiguration

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração de Registro de Dispositivo que restringe o número de dispositivos que um usuário pode registrar


Herda de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceEnrollmentLimitConfigurations](../api/intune-onboarding-deviceenrollmentlimitconfiguration-list.md)|Conjunto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|Listar propriedades e relações de objetos de [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).|
|[Obter deviceEnrollmentLimitConfiguration](../api/intune-onboarding-deviceenrollmentlimitconfiguration-get.md)|[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|Ler propriedades e relações de objetos de [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).|
|[Criar deviceEnrollmentLimitConfiguration](../api/intune-onboarding-deviceenrollmentlimitconfiguration-create.md)|[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|Criar um novo objeto de [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).|
|[Excluir deviceEnrollmentLimitConfiguration](../api/intune-onboarding-deviceenrollmentlimitconfiguration-delete.md)|Nenhum|Excluir [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).|
|[Atualizar deviceEnrollmentLimitConfiguration](../api/intune-onboarding-deviceenrollmentlimitconfiguration-update.md)|[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|Atualizar as propriedades de um objeto de [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para a conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|displayName|String|O nome de exibição da configuração de registro do dispositivo Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|description|String|A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|prioridade|Int32|A prioridade é usada quando um usuário existe em vários grupos que recebem a configuração de registro. Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixa. Herdada do [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Data e hora de criação em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|versão|Int32|A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|limite|Int32|O número máximo de dispositivos que um usuário pode registrar|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|atribuições|Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentLimitConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "limit": 1024
}
```





