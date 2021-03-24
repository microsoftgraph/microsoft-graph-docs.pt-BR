---
title: Atualizar macOSSoftwareUpdateAccountSummary
description: Atualize as propriedades de um objeto macOSSoftwareUpdateAccountSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b2412c54b1576308e7861cd961b211ea9fdc09dd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129724"
---
# <a name="update-macossoftwareupdateaccountsummary"></a>Atualizar macOSSoftwareUpdateAccountSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto macOSSoftwareUpdateAccountSummary.](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto macOSSoftwareUpdateAccountSummary.](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|displayName|Cadeia de caracteres|O nome do relatório|
|deviceId|Cadeia de caracteres|A ID do dispositivo.|
|userId|Cadeia de caracteres|A ID do usuário.|
|deviceName|String|O nome do dispositivo.|
|userPrincipalName|Cadeia de caracteres|O nome principal do usuário|
|osVersion|String|A versão do sistema operacional.|
|successfulUpdateCount|Int32|Número de atualizações bem-sucedidas no dispositivo.|
|failedUpdateCount|Int32|Número de atualizações com falha no dispositivo.|
|totalUpdateCount|Int32|Número de atualizações totais no dispositivo.|
|lastUpdatedDateTime|DateTimeOffset|Última data em que o relatório deste dispositivo foi atualizado.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}
Content-type: application/json
Content-length: 453

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateAccountSummary",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "userPrincipalName": "User Principal Name value",
  "osVersion": "Os Version value",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 502

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateAccountSummary",
  "id": "64687d05-7d05-6468-057d-6864057d6864",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "userPrincipalName": "User Principal Name value",
  "osVersion": "Os Version value",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```




