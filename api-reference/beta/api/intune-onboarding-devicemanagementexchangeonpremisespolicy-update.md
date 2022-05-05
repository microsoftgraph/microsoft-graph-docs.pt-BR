---
title: Atualizar deviceManagementExchangeOnPremisesPolicy
description: Atualize as propriedades de um objeto deviceManagementExchangeOnPremisesPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 48e29ff78556cb0568076c928923e1685cc12d6e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206298"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a>Atualizar deviceManagementExchangeOnPremisesPolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|
|notificationContent|Binária|Texto de notificação que será enviado aos usuários em quarentena por esta política. Este é o HTML da matriz de bytes codificado em UTF8.|
|defaultAccessLevel|[deviceManagementExchangeAccessLevel](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|Estado de acesso padrão Exchange. Essa regra se aplica globalmente a toda a Exchange organização. Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.|
|accessRules|[Coleção deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)|A lista de regras de acesso do dispositivo Exchange. As regras de acesso se aplicam globalmente a toda a Exchange organização|
|knownDeviceClasses|[Coleção deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|A lista de classes de dispositivo conhecidas Exchange|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
Content-type: application/json
Content-length: 665

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 714

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "16e76336-6336-16e7-3663-e7163663e716",
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```




