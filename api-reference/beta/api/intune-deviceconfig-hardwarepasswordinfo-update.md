---
title: Atualizar hardwarePasswordInfo
description: Atualize as propriedades de um objeto hardwarePasswordInfo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ddf665416159661ee7cf512565822146c3343ae5
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348363"
---
# <a name="update-hardwarepasswordinfo"></a>Atualizar hardwarePasswordInfo

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de um [objeto hardwarePasswordInfo.](../resources/intune-deviceconfig-hardwarepasswordinfo.md)

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
PATCH /deviceManagement/hardwarePasswordInfo/{hardwarePasswordInfoId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto hardwarePasswordInfo.](../resources/intune-deviceconfig-hardwarepasswordinfo.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo das informações de senha de hardware|
|serialNumber|String|Número de série do dispositivo|
|currentPassword|String|Senha do dispositivo atual|
|previousPasswords|Coleção String|Lista de senhas de dispositivo anterior|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/hardwarePasswordInfo/{hardwarePasswordInfoId}
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
HTTP/1.1 200 OK
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




