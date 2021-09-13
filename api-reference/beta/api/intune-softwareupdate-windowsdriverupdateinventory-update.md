---
title: Atualizar windowsDriverUpdateInventory
description: Atualize as propriedades de um objeto windowsDriverUpdateInventory.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 90abc5dec10bed9998cf988783f4cdb9c67fef89
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59138509"
---
# <a name="update-windowsdriverupdateinventory"></a>Atualizar windowsDriverUpdateInventory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de um [objeto windowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)

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
PATCH /deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}/driverInventories/{windowsDriverUpdateInventoryId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto windowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)

A tabela a seguir mostra as propriedades necessárias ao criar [o windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A id do driver.|
|nome|Cadeia de caracteres|O nome do driver.|
|versão|String|A versão do driver.|
|fabricante|String|O fabricante do driver.|
|releaseDateTime|DateTimeOffset|A data de lançamento do driver.|
|driverClass|Cadeia de Caracteres|A classe do driver.|
|applicableDeviceCount|Int32|O número de dispositivos para os quais esse driver é aplicável.|
|approvalStatus|[driverApprovalStatus](../resources/intune-softwareupdate-driverapprovalstatus.md)|O status de aprovação desse driver. Os valores possíveis são: `needsReview`, `declined`, `approved`, `suspended`.|
|category|[driverCategory](../resources/intune-softwareupdate-drivercategory.md)|A categoria desse driver. Os valores possíveis são: `recommended`, `previouslyApproved`, `other`.|
|deployDateTime|DateTimeOffset|A data em que um driver deve ser implantado se approvalStatus for aprovado.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}/driverInventories/{windowsDriverUpdateInventoryId}
Content-type: application/json
Content-length: 425

{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateInventory",
  "name": "Name value",
  "version": "Version value",
  "manufacturer": "Manufacturer value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "driverClass": "Driver Class value",
  "applicableDeviceCount": 5,
  "approvalStatus": "declined",
  "category": "previouslyApproved",
  "deployDateTime": "2017-01-01T00:01:14.7822152-08:00"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 474

{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateInventory",
  "id": "3b14b403-b403-3b14-03b4-143b03b4143b",
  "name": "Name value",
  "version": "Version value",
  "manufacturer": "Manufacturer value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "driverClass": "Driver Class value",
  "applicableDeviceCount": 5,
  "approvalStatus": "declined",
  "category": "previouslyApproved",
  "deployDateTime": "2017-01-01T00:01:14.7822152-08:00"
}
```



