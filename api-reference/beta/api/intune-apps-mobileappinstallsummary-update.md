---
title: Atualizar mobileAppInstallSummary
description: Atualize as propriedades de um objeto mobileAppInstallSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 19bd1e61359c5d2bdaff6ee87e807bae7dba0f05
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864796"
---
# <a name="update-mobileappinstallsummary"></a>Atualizar mobileAppInstallSummary

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Atualize as propriedades de um objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .

A tabela a seguir mostra as propriedades que são necessárias quando você cria o [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|installedDeviceCount|Int32|Número de dispositivos que instalou com sucesso deste aplicativo.|
|failedDeviceCount|Int32|Número de dispositivos que não tenha conseguido instalar esse aplicativo.|
|notApplicableDeviceCount|Int32|Número de dispositivos que não são aplicáveis para esse aplicativo.|
|notInstalledDeviceCount|Int32|Número de dispositivos que não tem este aplicativo instalado.|
|pendingInstallDeviceCount|Int32|Número de dispositivos que foram notificados para instalar esse aplicativo.|
|installedUserCount|Int32|Número de usuários cujos dispositivos tiveram êxito para instalar esse aplicativo.|
|failedUserCount|Int32|Número de usuários que têm 1 ou mais dispositivo com falha para instalar esse aplicativo.|
|notApplicableUserCount|Int32|Número de usuários cujos dispositivos tudo não eram aplicáveis para esse aplicativo.|
|notInstalledUserCount|Int32|Número de usuários que têm 1 ou mais dispositivos que não tiver instalado esse aplicativo.|
|pendingInstallUserCount|Int32|Número de usuários que têm 1 ou mais dispositivo que foram notificados para instalar esse aplicativo e tiver 0 dispositivos com falhas.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 312

{
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "06a792e9-92e9-06a7-e992-a706e992a706",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```





