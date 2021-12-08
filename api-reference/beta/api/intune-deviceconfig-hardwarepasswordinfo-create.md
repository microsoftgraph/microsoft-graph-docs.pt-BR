---
title: Criar hardwarePasswordInfo
description: Crie um novo objeto hardwarePasswordInfo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7477963532955ae66a397edae92c2a697ef25a6c
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345336"
---
# <a name="create-hardwarepasswordinfo"></a>Criar hardwarePasswordInfo

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto hardwarePasswordInfo.](../resources/intune-deviceconfig-hardwarepasswordinfo.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
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
POST /deviceManagement/hardwarePasswordInfo
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto hardwarePasswordInfo.

A tabela a seguir mostra as propriedades necessárias ao criar o hardwarePasswordInfo.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo das informações de senha de hardware|
|serialNumber|String|Número de série do dispositivo|
|currentPassword|String|Senha do dispositivo atual|
|previousPasswords|Coleção String|Lista de senhas de dispositivo anterior|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/hardwarePasswordInfo
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.hardwarePasswordInfo",
  "serialNumber": "Serial Number value",
  "currentPassword": "Current Password value",
  "previousPasswords": [
    "Previous Passwords value"
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 265

{
  "@odata.type": "#microsoft.graph.hardwarePasswordInfo",
  "id": "418e4bb4-4bb4-418e-b44b-8e41b44b8e41",
  "serialNumber": "Serial Number value",
  "currentPassword": "Current Password value",
  "previousPasswords": [
    "Previous Passwords value"
  ]
}
```




