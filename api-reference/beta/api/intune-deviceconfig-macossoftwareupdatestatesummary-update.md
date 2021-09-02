---
title: Atualizar macOSSoftwareUpdateStateSummary
description: Atualize as propriedades de um objeto macOSSoftwareUpdateStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82dcae148099204b599e31e05e583dd061f3d422
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58804187"
---
# <a name="update-macossoftwareupdatestatesummary"></a>Atualizar macOSSoftwareUpdateStateSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries/{macOSSoftwareUpdateStateSummaryId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|displayName|Cadeia de caracteres|Nome acessível humano da atualização de software|
|productKey|String|Chave do produto da atualização de software.|
|updateCategory|[macOSSoftwareUpdateCategory](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|Categoria de atualização de software. Os valores possíveis são: `critical`, `configurationDataFile`, `firmware`, `other`.|
|updateVersion|Cadeia de caracteres|Versão da atualização de software|
|state|[macOSSoftwareUpdateState](../resources/intune-deviceconfig-macossoftwareupdatestate.md)|Estado da atualização de software. Os valores possíveis são: `success` , , , , , , , , , `downloading` , , `downloaded` , , , `installing` `idle` `available` , `scheduled` `downloadFailed` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `installInsufficientSpace` `installInsufficientPower` `installFailed` `commandFailed` .|
|lastUpdatedDateTime|DateTimeOffset|Última data em que o relatório para este dispositivo e a chave do produto foi atualizado.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries/{macOSSoftwareUpdateStateSummaryId}
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
  "displayName": "Display Name value",
  "productKey": "Product Key value",
  "updateCategory": "configurationDataFile",
  "updateVersion": "Update Version value",
  "state": "downloading",
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
  "id": "9527a1df-a1df-9527-dfa1-2795dfa12795",
  "displayName": "Display Name value",
  "productKey": "Product Key value",
  "updateCategory": "configurationDataFile",
  "updateVersion": "Update Version value",
  "state": "downloading",
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```



