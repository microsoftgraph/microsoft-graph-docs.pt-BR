---
title: Criar termsAndConditionsAcceptanceStatus
description: Cria um novo objeto termsAndConditionsAcceptanceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ccfeefbce49404fb947c327501d7d6a36c1b93f
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734568"
---
# <a name="create-termsandconditionsacceptancestatus"></a>Criar termsAndConditionsAcceptanceStatus

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Cria um novo objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditionsAcceptanceStatus.

A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditionsAcceptanceStatus.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da entidade.|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário cuja aceitação a entidade representa.|
|acceptedVersion|Int32|Número da versão mais recente dos T&C aceitos pelo usuário.|
|acceptedDateTime|DateTimeOffset|A data e a hora em que os termos foram aceitos pela última vez pelo usuário.|
|userPrincipalName|String|O userPrincipalName do usuário que aceitou o termo.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 264

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00",
  "userPrincipalName": "User Principal Name value"
}
```





