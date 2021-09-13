---
title: Criar chromeOSOnboardingSettings
description: Crie um novo objeto chromeOSOnboardingSettings.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6a7200f79be8647c127135ae471a23d155f4d3d2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59112990"
---
# <a name="create-chromeosonboardingsettings"></a>Criar chromeOSOnboardingSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/chromeOSOnboardingSettings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto chromeOSOnboardingSettings.

A tabela a seguir mostra as propriedades que são necessárias ao criar os chromeOSOnboardingSettings.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do ChromebookTenant|
|ownerUserPrincipalName|String|OwnerUserPrincipalName do ChromebookTenant|
|onboardingStatus|[onboardingStatus](../resources/intune-chromebooksync-onboardingstatus.md)|OnboardingStatus do ChromebookTenant. Os valores possíveis são: `unknown`, `inprogress`, `onboarded`, `failed`.|
|lastModifiedDateTime|DateTimeOffset|LastModifiedDateTime do ChromebookTenant|
|lastDirectorySyncDateTime|DateTimeOffset|LastDirectorySyncDateTime do ChromebookTenant|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/chromeOSOnboardingSettings
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "onboardingStatus": "inprogress",
  "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 351

{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "id": "0344255d-255d-0344-5d25-44035d254403",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "onboardingStatus": "inprogress",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
}
```



