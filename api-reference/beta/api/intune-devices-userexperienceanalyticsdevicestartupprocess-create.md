---
title: Criar userExperienceAnalyticsDeviceStartupProcess
description: Criar um novo objeto userExperienceAnalyticsDeviceStartupProcess.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5b7c9e1eca9c70e65b1844071d22650a8de33c28
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082564"
---
# <a name="create-userexperienceanalyticsdevicestartupprocess"></a>Criar userExperienceAnalyticsDeviceStartupProcess

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsDeviceStartupProcess.

A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsDeviceStartupProcess.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do processo de inicialização do dispositivo de análise da experiência do usuário.|
|managedDeviceId|Cadeia de caracteres|A ID do dispositivo de análise da experiência do usuário.|
|Process|Cadeia de caracteres|Nome do processo de inicialização do dispositivo de análise da experiência do usuário.|
|productName|Cadeia de caracteres|O nome do produto do processo de inicialização do dispositivo analítico da experiência do usuário.|
|publicador|String|O fornecedor da experiência do usuário do processo de inicialização do dispositivo de análise.|
|startupImpactInMs|Int32|Impacto do processo de inicialização do dispositivo de análise de experiência do usuário em milissegundos.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
Content-type: application/json
Content-length: 276

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "managedDeviceId": "Managed Device Id value",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "startupImpactInMs": 1
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 325

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "id": "03b451e6-51e6-03b4-e651-b403e651b403",
  "managedDeviceId": "Managed Device Id value",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "startupImpactInMs": 1
}
```






