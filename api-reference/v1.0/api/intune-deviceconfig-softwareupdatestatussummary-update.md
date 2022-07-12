---
title: Atualizar softwareUpdateStatusSummary
description: Atualizar as propriedades de um objeto softwareUpdateStatusSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee4f4acf5bc61dfe81f3ab9b5a12de996c24ee5a
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66729675"
---
# <a name="update-softwareupdatestatussummary"></a>Atualizar softwareUpdateStatusSummary

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualizar as propriedades de um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).

A tabela a seguir mostra as propriedades obrigatórias ao criar [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|displayName|String|O nome da política.|
|compliantDeviceCount|Int32|Número de dispositivos em conformidade.|
|nonCompliantDeviceCount|Int32|Número de dispositivos sem conformidade.|
|remediatedDeviceCount|Int32|Número de dispositivos corrigidos.|
|errorDeviceCount|Int32|Número de dispositivos com erro.|
|unknownDeviceCount|Int32|Número de dispositivos desconhecidos.|
|conflictDeviceCount|Int32|Número de dispositivos em conflito.|
|notApplicableDeviceCount|Int32|Número de dispositivos não aplicáveis.|
|compliantUserCount|Int32|Número de usuários em conformidade.|
|nonCompliantUserCount|Int32|Número de usuários em não conformidade.|
|remediatedUserCount|Int32|Número de usuários corrigidos.|
|errorUserCount|Int32|Número de usuários com erro.|
|unknownUserCount|Int32|Número de usuários desconhecidos.|
|conflictUserCount|Int32|Número de usuários com conflitos.|
|notApplicableUserCount|Int32|Número de usuários não aplicáveis.|



## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```





