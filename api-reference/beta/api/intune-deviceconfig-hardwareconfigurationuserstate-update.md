---
title: Atualizar hardwareConfigurationUserState
description: Atualize as propriedades de um objeto hardwareConfigurationUserState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 866048d91807ce74cb6c65f12c4330e096c77355
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/04/2022
ms.locfileid: "61712016"
---
# <a name="update-hardwareconfigurationuserstate"></a>Atualizar hardwareConfigurationUserState

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto hardwareConfigurationUserState.](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)

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
PATCH /deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/userRunStates/{hardwareConfigurationUserStateId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto hardwareConfigurationUserState.](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade de estado do usuário do script de configuração de hardware. Essa propriedade é somente leitura.|
|upn|Cadeia de caracteres|Nome principal do usuário (UPN).|
|userEmail|Cadeia de caracteres|Endereço de Email do Usuário.|
|userName|Cadeia de caracteres|Nome de usuário|
|lastStateUpdateDateTime|DateTimeOffset|Last timestamp when the hardware configuration executed|
|successfulDeviceCount|Int32|Contagem de dispositivos de sucesso para usuários específicos.|
|failedDeviceCount|Int32|Contagem de dispositivos com falha para um usuário específico.|
|pendingDeviceCount|Int32|Contagem de dispositivos pendente para um usuário específico.|
|errorDeviceCount|Int32|Contagem de dispositivos de erro para usuário específico.|
|notApplicableDeviceCount|Int32|Contagem de dispositivos não aplicável para um usuário específico.|
|unknownDeviceCount|Int32|Contagem de dispositivos desconhecidos para usuários específicos.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/userRunStates/{hardwareConfigurationUserStateId}
Content-type: application/json
Content-length: 406

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationUserState",
  "upn": "Upn value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "successfulDeviceCount": 5,
  "failedDeviceCount": 1,
  "pendingDeviceCount": 2,
  "errorDeviceCount": 0,
  "notApplicableDeviceCount": 8,
  "unknownDeviceCount": 2
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 455

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationUserState",
  "id": "303ad215-d215-303a-15d2-3a3015d23a30",
  "upn": "Upn value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "successfulDeviceCount": 5,
  "failedDeviceCount": 1,
  "pendingDeviceCount": 2,
  "errorDeviceCount": 0,
  "notApplicableDeviceCount": 8,
  "unknownDeviceCount": 2
}
```




