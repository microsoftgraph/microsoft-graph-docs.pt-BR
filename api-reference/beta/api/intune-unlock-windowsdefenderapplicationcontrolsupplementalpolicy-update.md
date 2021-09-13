---
title: Atualizar windowsDefenderApplicationControlSupplementalPolicy
description: Atualize as propriedades de um objeto windowsDefenderApplicationControlSupplementalPolicy.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a53b4f9a9a1460cf5c58d0fecf62eb55b1e58cd2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59047881"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicy"></a>Atualizar windowsDefenderApplicationControlSupplementalPolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de um [objeto windowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}/policy
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto windowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave para a política suplementar WindowsDefenderApplicationControl.|
|displayName|Cadeia de caracteres|O nome de exibição da política suplementar WindowsDefenderApplicationControl.|
|description|Cadeia de caracteres|A descrição da política suplementar WindowsDefenderApplicationControl.|
|conteúdo|Binário|O conteúdo da política suplementar WindowsDefenderApplicationControl no formato de matriz de byte.|
|contentFileName|Cadeia de Caracteres|O nome do arquivo do conteúdo da política suplementar WindowsDefenderApplicationControl.|
|versão|String|A versão da política suplementar WindowsDefenderApplicationControl.|
|creationDateTime|DateTimeOffset|A data e a hora em que a política suplementar WindowsDefenderApplicationControl foi carregada.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a política suplementar WindowsDefenderApplicationControl foi modificada pela última vez.|
|roleScopeTagIds|String collection|Lista de Marcas de Escopo para esta entidade de política suplementar WindowsDefenderApplicationControl.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 517

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "id": "83d0c39e-c39e-83d0-9ec3-d0839ec3d083",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```



