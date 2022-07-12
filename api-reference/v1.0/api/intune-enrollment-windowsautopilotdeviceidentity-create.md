---
title: Criar windowsAutopilotDeviceIdentity
description: Crie um novo objeto windowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5875ec65c666b6cb4d04573181e22a022e63cfbe
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732832"
---
# <a name="create-windowsautopilotdeviceidentity"></a>Criar windowsAutopilotDeviceIdentity

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto windowsAutopilotDeviceIdentity.

A tabela a seguir mostra as propriedades que são necessárias ao criar windowsAutopilotDeviceIdentity.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O GUID do objeto.|
|groupTag|String|Marca de grupo do dispositivo windows autopilot.|
|purchaseOrderIdentifier|String|Identificador do Pedido de Compra do dispositivo Windows Autopilot.|
|serialNumber|Cadeia de caracteres|Número de série do dispositivo do Windows AutoPilot.|
|productKey|Cadeia de caracteres|Chave do produto (Product Key) do dispositivo do Windows AutoPilot.|
|fabricante|String|Fabricante OEM do dispositivo Windows Autopilot.|
|modelo|String|Nome do modelo do dispositivo Windows Autopilot.|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Intune estado de registro do dispositivo Windows Autopilot. Os valores possíveis são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`.|
|lastContactedDateTime|DateTimeOffset|Intune Data e Hora do Último Contato do dispositivo Windows Autopilot.|
|addressableUserName|String|Nome de usuário enderecável.|
|userPrincipalName|String|Nome UPN.|
|resourceName|Cadeia de caracteres|Nome do recurso.|
|skuNumber|String|Número da SKU|
|systemFamily|String|Família do Sistema|
|azureActiveDirectoryDeviceId|String|ID do dispositivo do AAD – a ser preterido|
|managedDeviceId|String|ID do Dispositivo Gerenciado|
|displayName|String|Nome de exibição|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `201 Created` de resposta e um [objeto windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 814

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "groupTag": "Group Tag value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 863

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "groupTag": "Group Tag value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```





