---
title: Criar groupPolicyOperation
description: Crie um novo objeto groupPolicyOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: add3c8bdacfd4bff56fea488f38ff1638afab267
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805868"
---
# <a name="create-grouppolicyoperation"></a>Criar groupPolicyOperation

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto groupPolicyOperation.](../resources/intune-grouppolicy-grouppolicyoperation.md)

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
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyOperation.

A tabela a seguir mostra as propriedades que são necessárias ao criar o groupPolicyOperation.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|operationType|[groupPolicyOperationType](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|O tipo de operação de política de grupo. Os valores possíveis são: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.|
|operationStatus|[groupPolicyOperationStatus](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|O status da operação de política de grupo. Os valores possíveis são: `unknown`, `inProgress`, `success`, `failed`.|
|statusDetails|Cadeia de caracteres|O detalhe do status da operação de política de grupo.|
|id|Cadeia de caracteres|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "upload",
  "operationStatus": "inProgress",
  "statusDetails": "Status Details value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "upload",
  "operationStatus": "inProgress",
  "statusDetails": "Status Details value",
  "id": "4d18865b-865b-4d18-5b86-184d5b86184d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



