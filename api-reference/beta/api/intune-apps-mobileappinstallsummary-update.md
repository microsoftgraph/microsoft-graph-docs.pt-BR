---
title: Atualizar mobileAppInstallSummary
description: Atualize as propriedades de um objeto mobileAppInstallSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 56e6a5379fec6cbbf25cb902df4ca2fca081884f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58756359"
---
# <a name="update-mobileappinstallsummary"></a>Atualizar mobileAppInstallSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de um [objeto mobileAppInstallSummary.](../resources/intune-apps-mobileappinstallsummary.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementApps.ReadWrite.All|

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
No corpo da solicitação, fornece uma representação JSON para o [objeto mobileAppInstallSummary.](../resources/intune-apps-mobileappinstallsummary.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|installedDeviceCount|Int32|Número de dispositivos que instalaram com êxito este aplicativo.|
|failedDeviceCount|Int32|Número de dispositivos que falharam ao instalar esse aplicativo.|
|notApplicableDeviceCount|Int32|Número de dispositivos que não são aplicáveis para este aplicativo.|
|notInstalledDeviceCount|Int32|Número de dispositivos que não têm esse aplicativo instalado.|
|pendingInstallDeviceCount|Int32|Número de dispositivos que foram notificados para instalar este aplicativo.|
|installedUserCount|Int32|Número de usuários cujos dispositivos foram todos bem-sucedidos para instalar este aplicativo.|
|failedUserCount|Int32|Número de usuários que têm 1 ou mais dispositivos que falharam ao instalar esse aplicativo.|
|notApplicableUserCount|Int32|Número de usuários cujos dispositivos não eram aplicáveis para este aplicativo.|
|notInstalledUserCount|Int32|Número de usuários que têm 1 ou mais dispositivos que não instalaram esse aplicativo.|
|pendingInstallUserCount|Int32|Número de usuários que têm 1 ou mais dispositivos que foram notificados para instalar esse aplicativo e têm 0 dispositivos com falhas.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
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



