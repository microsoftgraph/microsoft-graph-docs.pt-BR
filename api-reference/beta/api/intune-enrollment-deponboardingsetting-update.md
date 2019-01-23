---
title: Atualizar depOnboardingSetting
description: Atualize as propriedades de um objeto depOnboardingSetting.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 78d3138950776dd74a055fbb00339e9e69b5f0f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412286"
---
# <a name="update-deponboardingsetting"></a>Atualizar depOnboardingSetting

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Atualize as propriedades de um objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .

A tabela a seguir mostra as propriedades que são necessárias quando você cria o [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O UUID do objeto.|
|appleIdentifier|Cadeia de caracteres|A ID do Apple usada para obter o token atual.|
|tokenExpirationDateTime|DateTimeOffset|Quando o token irá expirar.|
|lastModifiedDateTime|DateTimeOffset|Quando o serviço foi onboarded.|
|lastSuccessfulSyncDateTime|DateTimeOffset|Quando o syned última do serviço com Intune|
|lastSyncTriggeredDateTime|DateTimeOffset|Quando o Intune solicitado último uma sincronização.|
|shareTokenWithSchoolDataSyncService|Boolean|Ou não o compartilhamento token do Dep está habilitado com o serviço de sincronização de dados da escola.|
|lastSyncErrorCode|Int32|Código de erro relatado pelo Apple durante a última sincronização dep.|
|tokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md)|Obtém ou define o tipo de Token do Dep. Os valores possíveis são: `none`, `dep`, `appleSchoolManager`.|
|tokenName|String|Nome amigável para o Token de Dep|
|syncedDeviceCount|Int32|Obtém sincronizados contagem de dispositivo|
|dataSharingConsentGranted|Boolean|Concedido consentimento para o compartilhamento de dados com Apple Dep Service|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 514

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 627

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "40342229-2229-4034-2922-344029223440",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true
}
```




