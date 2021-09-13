---
title: Tipo de recurso deviceManagementExchangeOnPremisesPolicy
description: Entidade Singleton que representa a política Exchange OnPremises configurada para um locatário.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d093fba796103d78e2691ef4177d98fb4c76947
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080818"
---
# <a name="devicemanagementexchangeonpremisespolicy-resource-type"></a>Tipo de recurso deviceManagementExchangeOnPremisesPolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade Singleton que representa a política Exchange OnPremises configurada para um locatário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagementExchangeOnPremisesPolicy](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-get.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Leia propriedades e relações do [objeto deviceManagementExchangeOnPremisesPolicy.](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|
|[Atualizar deviceManagementExchangeOnPremisesPolicy](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-update.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Atualize as propriedades de [um objeto deviceManagementExchangeOnPremisesPolicy.](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|
|notificationContent|Binário|Texto de notificação que será enviado aos usuários em quarentena por esta política. Este é o HTML da matriz de byte codificado UTF8.|
|defaultAccessLevel|[deviceManagementExchangeAccessLevel](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|Estado de acesso padrão Exchange. Essa regra se aplica globalmente a toda a Exchange organização. Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.|
|accessRules|[Coleção deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)|A lista de regras de acesso a dispositivos Exchange. As regras de acesso se aplicam globalmente a toda a Exchange organização|
|knownDeviceClasses|[Coleção deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|A lista de classes de dispositivo conhecidas Exchange|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|As configurações de acesso condicional do Exchange no local. O acesso condicional no local exigirá que os dispositivos sejam registrados e estejam em conformidade para o acesso ao email|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeOnPremisesPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "String (identifier)",
  "notificationContent": "binary",
  "defaultAccessLevel": "String",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "String",
        "type": "String"
      },
      "accessLevel": "String"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "String",
      "type": "String"
    }
  ]
}
```



