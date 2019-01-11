---
title: Atualizar androidForWorkSettings
description: Atualizar as propriedades de um objeto de androidForWorkSettings.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b46daa868d240b7ae50c83d708b8bf744e8079be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849760"
---
# <a name="update-androidforworksettings"></a>Atualizar androidForWorkSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Atualizar as propriedades de um objeto de [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).

A tabela a seguir mostra as propriedades obrigatórias ao criar [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de configurações do Android for Work|
|bindStatus|[androidForWorkBindStatus](../resources/intune-androidforwork-androidforworkbindstatus.md)|Associe o status do inquilino com a API do EMM Google. Os valores possíveis são: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Hora da conclusão da última sincronização do aplicativo|
|lastAppSyncStatus|[androidForWorkSyncStatus](../resources/intune-androidforwork-androidforworksyncstatus.md)|Resultado da última sincronização de aplicativo. Os possíveis valores são: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|Cadeia de caracteres|UPN proprietária que criou a empresa|
|ownerOrganizationName|Cadeia de caracteres|Nome da organização usada ao integrar o Android for Work|
|lastModifiedDateTime|DateTimeOffset|Hora da última modificação das configurações do Android for Work|
|enrollmentTarget|[androidForWorkEnrollmentTarget](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|Indica quais usuários podem inscrever dispositivos no Android para gerenciamento de dispositivo de trabalho. Os valores possíveis são: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|String collection|Especifica a quais grupos AAD podem registrar dispositivos no gerenciamento de dispositivos do Android for Work se enrollmentTarget estiver definido como 'Direcionado'|
|deviceOwnerManagementEnabled|Booliano|Indica se essa conta é flighting para o gerenciamento de proprietário de dispositivo Android com CloudDPC.|



## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 458

{
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 568

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```





