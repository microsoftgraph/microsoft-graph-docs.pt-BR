---
title: Criar windowsInformationProtectionDeviceRegistration
description: Crie um novo objeto windowsInformationProtectionDeviceRegistration.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c322453fc482f58d9551d82a34aa3473080dbb65
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59087754"
---
# <a name="create-windowsinformationprotectiondeviceregistration"></a>Criar windowsInformationProtectionDeviceRegistration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto windowsInformationProtectionDeviceRegistration.](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto windowsInformationProtectionDeviceRegistration.

A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionDeviceRegistration.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|userId|Cadeia de caracteres|UserId associado a esse registro de dispositivo.|
|deviceRegistrationId|Cadeia de caracteres|Identificador de dispositivo para esse registro de dispositivo.|
|deviceName|Cadeia de caracteres|Nome do dispositivo.|
|deviceType|String|Tipo de dispositivo, por exemplo, Windows laptop VS Windows telefone.|
|deviceMacAddress|Cadeia de Caracteres|Endereço do Device Mac.|
|lastCheckInDateTime|DateTimeOffset|Última verificação na hora do dispositivo.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations
Content-type: application/json
Content-length: 366

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 415

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "dd72e2c8-e2c8-dd72-c8e2-72ddc8e272dd",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```



