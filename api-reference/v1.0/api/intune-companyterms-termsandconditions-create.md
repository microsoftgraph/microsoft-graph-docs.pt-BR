---
title: Criar termsAndConditions
description: Criar um novo objeto termsAndConditions.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f2cd2350f3faa04883e3e65312b103c7cef96d41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835844"
---
# <a name="create-termsandconditions"></a>Criar termsAndConditions

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Criar um novo objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditions.

A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditions.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da política de T&C.|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado.|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto.|
|displayName|Cadeia de caracteres|Nome fornecido pelo administrador para a política de T&C. |
|description|Cadeia de caracteres|Descrição fornecida pelo administrador para a política de T&C.|
|title|Cadeia de caracteres|Título dos termos e condições fornecido pelo administrador. Isso é exibido ao usuário nos prompts de aceitação da política de T&C.|
|bodyText|Cadeia de caracteres|Corpo de texto de termos e condições fornecido pelo administrador, normalmente os termos em si. Isso é exibido ao usuário nos prompts de aceitação da política de T&C.|
|acceptanceStatement|Cadeia de caracteres|Explicação dos termos e condições fornecida pelo administrador, normalmente para descrever o que significa aceitar os termos e condições definidos na política de T&C. Isso é exibido ao usuário nos prompts de aceitação da política de T&C.|
|version|Int32|Inteiro que indica a versão atual dos termos. Incrementado quando um administrador faz uma alteração nos termos e deseja solicitar que os usuários aceitem novamente a política de T&C modificada.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 445

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```



