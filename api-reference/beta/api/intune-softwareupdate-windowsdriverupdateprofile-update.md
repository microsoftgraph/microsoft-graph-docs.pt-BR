---
title: Atualizar windowsDriverUpdateProfile
description: Atualize as propriedades de um objeto windowsDriverUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 58b4b986183f4ac5247103a8d214e7c488811cc2
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2022
ms.locfileid: "64629488"
---
# <a name="update-windowsdriverupdateprofile"></a>Atualizar windowsDriverUpdateProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de um [objeto windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A Intune de política.|
|displayName|String|O nome de exibição do perfil.|
|descrição|String|A descrição do perfil especificado pelo usuário.|
|approvalType|[driverUpdateProfileApprovalType](../resources/intune-softwareupdate-driverupdateprofileapprovaltype.md)|Tipo de aprovação de perfil de atualização de driver. Por exemplo, aprovação manual ou automática. Os valores possíveis são: `manual` e `automatic`.|
|deviceReporting|Int32|Número de dispositivos que relatam esse perfil|
|newUpdates|Int32|Número de novas atualizações de driver disponíveis para esse perfil.|
|deploymentDeferralInDays|Int32|Configurações de adiamento de implantação em dias, aplicável somente quando ApprovalType é definido como aprovação automática.|
|createdDateTime|DateTimeOffset|A data em que o perfil foi criado.|
|lastModifiedDateTime|DateTimeOffset|A data em que o perfil foi modificado pela última vez.|
|roleScopeTagIds|Conjunto de cadeias de caracteres|Lista de Marcas de Escopo para essa entidade de Atualização de Driver.|
|inventorySyncStatus|[windowsDriverUpdateProfileInventorySyncStatus](../resources/intune-softwareupdate-windowsdriverupdateprofileinventorysyncstatus.md)|Status de sincronização de inventário de driver para este perfil.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um [objeto windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}
Content-type: application/json
Content-length: 555

{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "approvalType": "automatic",
  "deviceReporting": 15,
  "newUpdates": 10,
  "deploymentDeferralInDays": 8,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "inventorySyncStatus": {
    "@odata.type": "microsoft.graph.windowsDriverUpdateProfileInventorySyncStatus",
    "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
    "driverInventorySyncState": "success"
  }
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 727

{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateProfile",
  "id": "55bcc52a-c52a-55bc-2ac5-bc552ac5bc55",
  "displayName": "Display Name value",
  "description": "Description value",
  "approvalType": "automatic",
  "deviceReporting": 15,
  "newUpdates": 10,
  "deploymentDeferralInDays": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "inventorySyncStatus": {
    "@odata.type": "microsoft.graph.windowsDriverUpdateProfileInventorySyncStatus",
    "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
    "driverInventorySyncState": "success"
  }
}
```




