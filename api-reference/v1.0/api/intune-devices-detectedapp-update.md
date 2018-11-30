---
title: Atualizar detectedApp
description: Atualizar as propriedades de um objeto detectedApp.
ms.openlocfilehash: b35a5ba7da0dc02d97a63d7a80aa304707b326a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004234"
---
# <a name="update-detectedapp"></a>Atualizar detectedApp

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Atualizar as propriedades de um objeto [detectedApp](../resources/intune-devices-detectedapp.md).
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Accept|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [detectedApp](../resources/intune-devices-detectedapp.md).

A tabela a seguir mostra as propriedades que são necessárias ao criar [detectedApp](../resources/intune-devices-detectedapp.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do aplicativo detectado. Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado. Somente leitura.|
|displayName|Cadeia de caracteres|Nome do aplicativo descoberto. Somente leitura|
|version|Cadeia de caracteres|Versão do aplicativo descoberto. Somente leitura|
|sizeInByte|Int64|Tamanho do aplicativo descoberto, em bytes. Somente leitura|
|deviceCount|Int32|O número de dispositivos que instalaram esse aplicativo|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [detectedApp](../resources/intune-devices-detectedapp.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}
Content-type: application/json
Content-length: 167

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 216

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```



