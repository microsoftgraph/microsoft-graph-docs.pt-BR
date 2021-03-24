---
title: Atualizar securityBaselineCategoryStateSummary
description: Atualize as propriedades de um objeto securityBaselineCategoryStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af9b11acf7d5bbf7fe4a4aafd517a8b589abf23e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131999"
---
# <a name="update-securitybaselinecategorystatesummary"></a>Atualizar securityBaselineCategoryStateSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)

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
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para [o objeto securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da entidade. Herdado [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|secureCount|Int32|Número de dispositivos seguros Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|notSecureCount|Int32|Número de dispositivos não seguros Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|unknownCount|Int32|Número de dispositivos desconhecidos Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|errorCount|Int32|Número de dispositivos de erro Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|conflictCount|Int32|Número de dispositivos de conflito Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|notApplicableCount|Int32|Número de dispositivos não aplicáveis Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|displayName|Cadeia de caracteres|O nome da categoria|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "7a650997-0997-7a65-9709-657a9709657a",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```




