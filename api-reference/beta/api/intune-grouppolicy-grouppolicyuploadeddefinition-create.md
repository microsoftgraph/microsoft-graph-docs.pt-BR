---
title: Criar groupPolicyUploadedDefinition
description: Crie um novo objeto groupPolicyUploadedDefinition.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1e532cd55cf0271ddea3b8244fddd31fa1066be3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59041959"
---
# <a name="create-grouppolicyuploadeddefinition"></a>Criar groupPolicyUploadedDefinition

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto groupPolicyUploadedDefinition.](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)

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
POST /deviceManagement/groupPolicyDefinitions
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitions
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyUploadedDefinition.

A tabela a seguir mostra as propriedades que são necessárias ao criar o groupPolicyUploadedDefinition.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|Identifica o tipo de grupos aos qual a política pode ser aplicada. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md). Os valores possíveis são: `user` e `machine`.|
|displayName|Cadeia de caracteres|O nome da política localizada. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|explainText|Cadeia de Caracteres|A explicação localizada ou o texto de ajuda associado à política. O valor padrão é vazio. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|categoryPath|Cadeia de Caracteres|O caminho de categoria completa localizado para a política. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|supportedOn|Cadeia de Caracteres|Cadeia de caracteres localizada usada para especificar qual versão do sistema operacional ou aplicativo é afetada pela política. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Especifica o tipo de política de grupo. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md). Os valores possíveis são: `admxBacked` e `admxIngested`.|
|hasRelatedDefinitions|Boleano|Significa se há ou não definições relacionadas a essa definição Herdadas de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|groupPolicyCategoryId|Guid|A id de categoria da categoria pai Herdada de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|minDeviceCspVersion|Cadeia de Caracteres|Versão mínima necessária do CSP para configuração do dispositivo nesta definição Herdada de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|minUserCspVersion|Cadeia de Caracteres|Versão mínima necessária do CSP para configuração do usuário nesta definição Herdada de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|versão|String|Definindo a versão de definição Herdada [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions
Content-type: application/json
Content-length: 538

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "hasRelatedDefinitions": true,
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
  "minDeviceCspVersion": "Min Device Csp Version value",
  "minUserCspVersion": "Min User Csp Version value",
  "version": "Version value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "hasRelatedDefinitions": true,
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
  "minDeviceCspVersion": "Min Device Csp Version value",
  "minUserCspVersion": "Min User Csp Version value",
  "version": "Version value",
  "id": "a5f83119-3119-a5f8-1931-f8a51931f8a5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



