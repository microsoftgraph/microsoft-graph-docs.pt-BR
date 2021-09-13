---
title: Criar groupPolicyUploadedDefinitionFile
description: Crie um novo objeto groupPolicyUploadedDefinitionFile.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aae0b137d590c65005ff1a849ab2d92019bab1ee
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59041917"
---
# <a name="create-grouppolicyuploadeddefinitionfile"></a>Criar groupPolicyUploadedDefinitionFile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto groupPolicyUploadedDefinitionFile.](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
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
POST /deviceManagement/groupPolicyUploadedDefinitionFiles
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyUploadedDefinitionFile.

A tabela a seguir mostra as propriedades que são necessárias ao criar o groupPolicyUploadedDefinitionFile.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome amigável localizado do arquivo ADMX. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|description|Cadeia de caracteres|A descrição localizada das configurações de política no arquivo ADMX. O valor padrão é vazio. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|languageCodes|String collection|Os códigos de idioma com suporte para o arquivo ADMX. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|targetPrefix|Cadeia de Caracteres|Especifica o nome lógico que se refere ao namespace no arquivo ADMX. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|targetNamespace|Cadeia de Caracteres|Especifica o URI usado para identificar o namespace no arquivo ADMX. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Especifica o tipo de política de grupo. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md). Os valores possíveis são: `admxBacked` e `admxIngested`.|
|revision|Cadeia de Caracteres|A versão de revisão associada ao arquivo. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado [de groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|fileName|String|O nome do arquivo ADML carregado.|
|status|[groupPolicyUploadedDefinitionFileStatus](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfilestatus.md)|O status de carregamento do arquivo ADMX carregado. Os valores possíveis são: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.|
|conteúdo|Binário|O conteúdo do arquivo ADMX carregado.|
|uploadDateTime|DateTimeOffset|O tempo carregado do arquivo ADMX carregado.|
|defaultLanguageCode|Cadeia de Caracteres|O idioma padrão do arquivo ADMX carregado.|
|groupPolicyUploadedLanguageFiles|[coleção groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)|A lista de arquivos ADML associados ao arquivo ADMX carregado.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles
Content-type: application/json
Content-length: 922

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value",
  "fileName": "File Name value",
  "status": "uploadInProgress",
  "content": "Y29udGVudA==",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00",
  "defaultLanguageCode": "Default Language Code value",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "File Name value",
      "languageCode": "Language Code value",
      "content": "Y29udGVudA==",
      "id": "Id value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1035

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value",
  "id": "0ce1a8cf-a8cf-0ce1-cfa8-e10ccfa8e10c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "fileName": "File Name value",
  "status": "uploadInProgress",
  "content": "Y29udGVudA==",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00",
  "defaultLanguageCode": "Default Language Code value",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "File Name value",
      "languageCode": "Language Code value",
      "content": "Y29udGVudA==",
      "id": "Id value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```



