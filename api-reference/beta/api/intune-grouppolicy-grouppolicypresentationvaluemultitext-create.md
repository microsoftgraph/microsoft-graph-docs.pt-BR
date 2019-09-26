---
title: Criar groupPolicyPresentationValueMultiText
description: Criar um novo objeto groupPolicyPresentationValueMultiText.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3accf2cde6856e09372d40be60bceecab9f43ecc
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37193568"
---
# <a name="create-grouppolicypresentationvaluemultitext"></a>Criar groupPolicyPresentationValueMultiText

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
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
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationValueMultiText.

A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationValueMultiText.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o objeto foi modificado pela última vez. Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|A data e a hora em que o objeto foi criado. Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|Chave da entidade. Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|values|Coleção de cadeias de caracteres|Uma coleção de cadeias de caracteres não vazias para a apresentação associada.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "values": [
    "Values value"
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 292

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "5156903b-903b-5156-3b90-56513b905651",
  "values": [
    "Values value"
  ]
}
```




