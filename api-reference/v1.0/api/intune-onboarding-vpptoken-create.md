---
title: Criar vppToken
description: Criar um novo objeto vppToken.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6e5715e3fea9b864a1b94d7747c8cd7477904f09
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60451469"
---
# <a name="create-vpptoken"></a>Criar vppToken

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [vppToken](../resources/intune-onboarding-vpptoken.md).

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
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto vppToken.

A tabela a seguir mostra as propriedades que são necessárias ao criar o vppToken.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Isso é gerado automaticamente quando o appleVolumePurchaseProgramToken é criado. É a Chave da entidade.|
|organizationName|Cadeia de caracteres|A organização associada ao Token do Programa de Compra por Volume da Apple|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado. Os valores possíveis são: `business`, `education`. Os valores possíveis são: `business`, `education`.|
|appleId|Cadeia de caracteres|O Apple ID associado ao Token do Apple Volume Purchase Program.|
|expirationDateTime|DateTimeOffset|A data e hora de expiração do Token do Apple Volume Purchase Program.|
|lastSyncDateTime|DateTimeOffset|A última vez que uma sincronização de aplicativo foi realizada com o serviço do Apple Volume Purchase Program usando o Token do Apple Volume Purchase Program.|
|token|Cadeia de caracteres|A cadeia de caracteres do Token do Apple Volume Purchase Program baixada do Apple Volume Purchase Program.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação associada com o Token do Apple Volume Purchase Program.|
|state|[vppTokenState](../resources/intune-onboarding-vpptokenstate.md)|Estado atual do Token do Apple Volume Purchase Program. Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune-onboarding-vpptokensyncstatus.md)|Status atual de sincronização da última sincronização de aplicativo que foi feita usando o Token do Apple Volume Purchase Program. Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`. Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.|
|automaticallyUpdateApps|Boolean|Se os aplicativos para o token VPP serão automaticamente atualizados ou não.|
|countryOrRegion|Cadeia de caracteres|Se os aplicativos para o token VPP serão automaticamente atualizados ou não.|



## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
Content-type: application/json
Content-length: 461

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```



