---
title: Criar microsoftTunnelSite
description: Crie um novo objeto microsoftTunnelSite.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ec24b6fb069300d85fee5b0d7dbf26e8f42548ee
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59096890"
---
# <a name="create-microsofttunnelsite"></a>Criar microsoftTunnelSite

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelSites
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto microsoftTunnelSite.

A tabela a seguir mostra as propriedades que são necessárias ao criar o microsoftTunnelSite.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Id do MicrosoftTunnelSite|
|displayName|Cadeia de caracteres|O nome de exibição do MicrosoftTunnelSite|
|description|Cadeia de caracteres|Descrição do MicrosoftTunnelSite|
|publicAddress|Cadeia de Caracteres|O nome de domínio público do MicrosoftTunnelSite ou o endereço IP|
|upgradeWindowUtcOffsetInMinutes|Int32|O timezone do site representado como um deslocamento de minuto do UTC|
|upgradeWindowStartTime|TimeOfDay|Hora de início da janela de atualização do site|
|upgradeWindowEndTime|TimeOfDay|Hora de término da janela de atualização do site|
|upgradeAutomatically|Boleano|A configuração de atualização automática do site. True para atualizações automáticas, false para controle manual|
|upgradeAvailable|Boleano|True se uma atualização estiver disponível|
|internalNetworkProbeUrl|Cadeia de Caracteres|A URL da Sonda de Acesso à Rede Interna do MicrosoftTunnelSite|
|roleScopeTagIds|String collection|Lista de marcas de escopo para esta instância entity.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites
Content-type: application/json
Content-length: 524

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "upgradeWindowUtcOffsetInMinutes": 15,
  "upgradeWindowStartTime": "12:01:27.3030000",
  "upgradeWindowEndTime": "11:57:17.9830000",
  "upgradeAutomatically": true,
  "upgradeAvailable": true,
  "internalNetworkProbeUrl": "https://example.com/internalNetworkProbeUrl/",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 573

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "id": "b2f7dc3e-dc3e-b2f7-3edc-f7b23edcf7b2",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "upgradeWindowUtcOffsetInMinutes": 15,
  "upgradeWindowStartTime": "12:01:27.3030000",
  "upgradeWindowEndTime": "11:57:17.9830000",
  "upgradeAutomatically": true,
  "upgradeAvailable": true,
  "internalNetworkProbeUrl": "https://example.com/internalNetworkProbeUrl/",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```



