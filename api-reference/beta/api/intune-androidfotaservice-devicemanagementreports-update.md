---
title: Atualizar deviceManagementReports
description: Atualize as propriedades de um objeto deviceManagementReports.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9075fa6a7291fa74094fa1bf86c10d0360cbf1c1
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858573"
---
# <a name="update-devicemanagementreports"></a>Atualizar deviceManagementReports

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto deviceManagementReports](../resources/intune-androidfotaservice-devicemanagementreports.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementReports](../resources/intune-androidfotaservice-devicemanagementreports.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementReports](../resources/intune-androidfotaservice-devicemanagementreports.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [deviceManagementReports](../resources/intune-androidfotaservice-devicemanagementreports.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```




