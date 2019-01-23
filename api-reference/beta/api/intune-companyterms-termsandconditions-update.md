---
title: Atualizar termsAndConditions
description: Atualizar as propriedades de um objeto termsAndConditions.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3eca58812eb4032113e968ad054a7a11bf110b81
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409486"
---
# <a name="update-termsandconditions"></a>Atualizar termsAndConditions

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Atualizar as propriedades de um objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).

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
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).

A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da política de T&C.|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado.|
|modifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto.|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto.|
|displayName|String|Nome fornecido pelo administrador para a política de T&C. |
|description|String|Descrição fornecida pelo administrador para a política de T&C.|
|title|String|Título dos termos e condições fornecido pelo administrador. Isso é exibido ao usuário nos prompts de aceitação da política de T&C.|
|bodyText|String|Corpo de texto de termos e condições fornecido pelo administrador, normalmente os termos em si. Isso é exibido ao usuário nos prompts de aceitação da política de T&C.|
|acceptanceStatement|String|Explicação dos termos e condições fornecida pelo administrador, normalmente para descrever o que significa aceitar os termos e condições definidos na política de T&C. Isso é exibido ao usuário nos prompts de aceitação da política de T&C.|
|version|Int32|Inteiro que indica a versão atual dos termos. Incrementado quando um administrador faz uma alteração nos termos e deseja solicitar que os usuários aceitem novamente a política de T&C modificada.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
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
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 505

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```




