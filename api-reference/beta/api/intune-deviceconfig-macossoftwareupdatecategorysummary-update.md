---
title: Atualizar macOSSoftwareUpdateCategorySummary
description: Atualize as propriedades de um objeto macOSSoftwareUpdateCategorySummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4a4fa5fa8fbfa64cc8e874823d08f3bf8df1d5dc0e7ea29780ca59d3e8686a2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54132239"
---
# <a name="update-macossoftwareupdatecategorysummary"></a>Atualizar macOSSoftwareUpdateCategorySummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)

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
PATCH /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|displayName|Cadeia de caracteres|O nome do relatório|
|deviceId|Cadeia de caracteres|A ID do dispositivo.|
|userId|Cadeia de caracteres|A ID do usuário.|
|updateCategory|[macOSSoftwareUpdateCategory](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|Tipo de atualização de software. Os valores possíveis são: `critical`, `configurationDataFile`, `firmware`, `other`.|
|successfulUpdateCount|Int32|Número de atualizações bem-sucedidas no dispositivo|
|failedUpdateCount|Int32|Número de atualizações com falha no dispositivo|
|totalUpdateCount|Int32|Número de atualizações totais no dispositivo|
|lastUpdatedDateTime|DateTimeOffset|Última data em que o relatório deste dispositivo foi atualizado.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}
Content-type: application/json
Content-length: 373

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateCategorySummary",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "updateCategory": "configurationDataFile",
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
Content-Length: 422

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateCategorySummary",
  "id": "f1fda232-a232-f1fd-32a2-fdf132a2fdf1",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "updateCategory": "configurationDataFile",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```




