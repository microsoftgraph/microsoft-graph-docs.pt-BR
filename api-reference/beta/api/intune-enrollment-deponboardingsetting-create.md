---
title: Criar depOnboardingSetting
description: Criar um novo objeto depOnboardingSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d605f4a18eab5eacb3e8c53070a721952c54f7cf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49201692"
---
# <a name="create-deponboardingsetting"></a>Criar depOnboardingSetting

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto depOnboardingSetting.

A tabela a seguir mostra as propriedades que são necessárias ao criar depOnboardingSetting.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O UUID do objeto.|
|appleIdentifier|Cadeia de caracteres|A ID da Apple usada para obter o token atual.|
|tokenExpirationDateTime|DateTimeOffset|Quando o token expirará.|
|lastModifiedDateTime|DateTimeOffset|Quando o serviço foi integrado.|
|lastSuccessfulSyncDateTime|DateTimeOffset|Quando o serviço última syned com o Intune|
|lastSyncTriggeredDateTime|DateTimeOffset|Quando o Intune solicitou uma sincronização pela última vez.|
|shareTokenWithSchoolDataSyncService|Booliano|Se o compartilhamento de token DEP está ou não habilitado com o serviço de sincronização de dados da escola.|
|lastSyncErrorCode|Int32|Código de erro relatado pela Apple durante a última sincronização de Dep.|
|TokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md)|Obtém ou define o tipo de token Dep. Os valores possíveis são: `none`, `dep`, `appleSchoolManager`.|
|tokenname|String|Nome amigável para token Dep|
|syncedDeviceCount|Int32|Obtém a contagem de dispositivos sincronizados|
|dataSharingConsentGranted|Booliano|Consentimento concedido para compartilhamento de dados com o serviço Apple Dep|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
Content-type: application/json
Content-length: 576

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
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 689

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
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




