---
title: Atualizar sideLoadingKey
description: Atualize as propriedades de um objeto sideLoadingKey.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4fd498404543353c45714f739a68b0195ae3d3dd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409857"
---
# <a name="update-sideloadingkey"></a>Atualizar sideLoadingKey

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Atualize as propriedades de um objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .

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
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .

A tabela a seguir mostra as propriedades que são necessárias quando você cria o [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Lado carregando o ID exclusivo principal.|
|valor|String|Valor da chave Carregando lado, é 5x5 valor, separados por hiphens.|
|displayName|String|Carregando da lado chave nome exibido para o ITPro Admins.|
|description|String|Descrição de chave Carregando lado exibida para o ITPro Admins..|
|totalActivation|Int32|Lado Carregando chave Total Activation exibida para o ITPro Admins.|
|lastUpdatedDateTime|String|Lado Carregando chave última atualizado data exibida para o ITPro Admins.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
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
HTTP/1.1 200 OK
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




