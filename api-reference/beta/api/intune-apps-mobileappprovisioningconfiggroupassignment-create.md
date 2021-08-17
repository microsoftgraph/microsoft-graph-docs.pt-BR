---
title: Criar mobileAppProvisioningConfigGroupAssignment
description: Crie um novo objeto mobileAppProvisioningConfigGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8d1c246066b728338629c41ef1c8da59c1340da889de36e9cbdb664e67072c53
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54204643"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a>Criar mobileAppProvisioningConfigGroupAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto mobileAppProvisioningConfigGroupAssignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto mobileAppProvisioningConfigGroupAssignment.

A tabela a seguir mostra as propriedades que são necessárias ao criar o mobileAppProvisioningConfigGroupAssignment.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|targetGroupId|Cadeia de caracteres|A ID do grupo AAD no qual a configuração de provisionamento de aplicativo está sendo direcionada.|
|id|Cadeia de caracteres|Chave da entidade.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```




