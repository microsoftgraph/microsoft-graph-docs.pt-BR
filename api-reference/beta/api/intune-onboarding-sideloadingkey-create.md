---
title: Criar sideLoadingKey
description: Crie um novo objeto sideLoadingKey.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5a484745aae11ba967f3077bf674c9bc8dd8c6db
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148740"
---
# <a name="create-sideloadingkey"></a>Criar sideLoadingKey

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)

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
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto sideLoadingKey.

A tabela a seguir mostra as propriedades que são necessárias ao criar o sideLoadingKey.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID exclusiva da chave de carregamento lateral.|
|value|Cadeia de caracteres|Side Loading Key Value, it is 5x5 value, seperated by hiphens.|
|displayName|Cadeia de caracteres|Side Loading Key Name displayed to the ITPro Admins.|
|descrição|Cadeia de caracteres|Descrição da Chave de Carregamento lateral exibida para os administradores do ITPro..|
|totalActivation|Int32|Side Loading Key Total Activation displayed to the ITPro Admins.|
|lastUpdatedDateTime|Cadeia de caracteres|Side Loading Key Last Updated Date displayed to the ITPro Admins.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```




