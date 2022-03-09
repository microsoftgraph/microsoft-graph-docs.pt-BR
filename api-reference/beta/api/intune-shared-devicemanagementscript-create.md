---
title: Criar deviceManagementScript
description: Crie um novo objeto deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 922acbdd39dafe63b21c815f38be4ed377817cf0
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367745"
---
# <a name="create-devicemanagementscript"></a>Criar deviceManagementScript

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)||
| &nbsp; &nbsp; **Gerenciamento de dispositivos** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp;&nbsp; **Conjunto de Políticas** | DeviceManagementManagedDevices.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo||
| &nbsp; &nbsp; **Gerenciamento de dispositivos** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp;&nbsp; **Conjunto de Políticas** | DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementScript.

A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScript.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do script de gerenciamento de dispositivos.|
|displayName|String|Nome do script de gerenciamento de dispositivos.|
|description|String|Descrição opcional para o script de gerenciamento de dispositivos.|
|scriptContent|Binária|O conteúdo do script.|
|createdDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivos foi criado. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivos foi modificado pela última vez. Essa propriedade é somente leitura.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução. Os valores possíveis são: `system` e `user`.|
|enforceSignatureCheck|Booliano|Indique se a assinatura de script precisa ser verificada.|
|fileName|String|Nome do arquivo de script.|
|roleScopeTagIds|String collection|Lista de IDs de marca de escopo para esta instância do PowerShellScript.|
|runAs32Bit|Booliano|Um valor que indica se o script do PowerShell deve ser executado como 32 bits|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201 Created` código de resposta e um [objeto deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 615

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```






