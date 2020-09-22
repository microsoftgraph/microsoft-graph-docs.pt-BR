---
title: Criar groupPolicyUploadedCategory
description: Criar um novo objeto groupPolicyUploadedCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fbe42b8da4c1b38e21be1daab555a4d7818ccdff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48068172"
---
# <a name="create-grouppolicyuploadedcategory"></a>Criar groupPolicyUploadedCategory

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyCategories
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/children
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyUploadedCategory.

A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyUploadedCategory.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|A ID da cadeia de caracteres do nome de exibição da categoria herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|IsRoot|Booliano|Define se a categoria é uma categoria raiz herdada de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
  "displayName": "Display Name value",
  "isRoot": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 241

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
  "displayName": "Display Name value",
  "isRoot": true,
  "id": "7e373e80-3e80-7e37-803e-377e803e377e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```






