---
title: Atualizar groupPolicyObjectFile
description: Atualiza as propriedades de um objeto groupPolicyObjectFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b266b110a0512539018815c0bf4f3cd33700fb3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692993"
---
# <a name="update-grouppolicyobjectfile"></a>Atualizar groupPolicyObjectFile

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualiza as propriedades de um objeto [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
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
PATCH /deviceManagement/groupPolicyObjectFiles/{groupPolicyObjectFileId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Ainda não documentado|
|groupPolicyObjectId|Guid|O GUID do objeto da política de grupo do conteúdo XML do GPO|
|ouDistinguishedName|String|O nome diferenciado da OU.|
|createdDateTime|DateTimeOffset|A data e a hora em que o GroupPolicy foi carregado pela primeira vez.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o GroupPolicyObjectFile foi modificado pela última vez.|
|content|Cadeia de caracteres|O conteúdo do arquivo do objeto de diretiva de grupo.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyObjectFiles/{groupPolicyObjectFileId}
Content-type: application/json
Content-length: 217

{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "content": "Content value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 389

{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "id": "65c0499d-499d-65c0-9d49-c0659d49c065",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "content": "Content value"
}
```





