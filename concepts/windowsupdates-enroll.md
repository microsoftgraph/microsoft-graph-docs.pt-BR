---
title: Registrar-se no gerenciamento de atualizações pelo serviço de implantação Windows Update para Empresas
description: Registre um dispositivo no gerenciamento de atualizações para que você possa usar o serviço de implantação do Windows Update for Business para gerenciar o conteúdo fornecido Windows Update para esse dispositivo.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 1606b9a063a11406366f63ae9d26add8ddded96b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437489"
---
# <a name="enroll-in-update-management-by-the-windows-update-for-business-deployment-service"></a>Registrar-se no gerenciamento de atualizações pelo serviço de implantação Windows Update para Empresas

Ao registrar um dispositivo no gerenciamento de atualizações pelo serviço de implantação do Windows Update for Business, você pode usar o serviço de implantação para gerenciar o conteúdo fornecido Windows Update para esse dispositivo. Você pode registrar um dispositivo no gerenciamento de atualizações por categoria de atualização.

Atualmente, o serviço de implantação dá suporte ao registro no gerenciamento de Windows 10 de recursos. No momento, o serviço de implantação não requer registro no gerenciamento de atualizações Windows 10 qualidade para implantar atualizações de qualidade aceleradas.

## <a name="enroll-the-device-in-update-management"></a>Registrar o dispositivo no gerenciamento de atualizações

Quando você registra um dispositivo no gerenciamento de uma determinada categoria de atualização, o serviço de implantação se torna a autoridade para atualizações dessa categoria provenientes de Windows Update. Como resultado, os dispositivos não recebem atualizações dessa categoria do Windows Update até que você implante uma atualização usando o serviço de implantação atribuindo-a a uma [implantação](windowsupdates-deployments.md). Os dispositivos são registrados automaticamente com o serviço quando registrados no gerenciamento pelo serviço (ou seja, um objeto [azureADDevice é criado automaticamente](/graph/api/resources/windowsupdates-azureaddevice) se ele ainda não existir).

### <a name="request"></a>Solicitação

``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/enrollAssets
Content-Type: application/json

{
  "updateCategory": "feature",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```

### <a name="response"></a>Resposta

``` http
HTTP/1.1 202 Accepted
```

## <a name="check-the-enrollment-state-of-a-device"></a>Verificar o estado de registro de um dispositivo

Você pode verificar o estado de registro de um dispositivo obtendo o dispositivo e examinando as  propriedades de registros  e erros no objeto **azureADDevice**.[](/graph/api/windowsupdates-azureaddevice-get) Um dispositivo registrado com êxito no gerenciamento de atualizações tem um objeto [updateManagementEnrollment](/graph/api/resources/windowsupdates-updatemanagementenrollment) na coleção de registros e não tem nenhum objeto [updatableAssetError](/graph/api/resources/windowsupdates-updatableasseterror) na coleção de erros. Um dispositivo que o serviço tentou registrar, mas encontrou um erro, preencheu coleções para registros e erros. Um dispositivo para o qual o serviço não recebeu nenhuma solicitação de registro tem coleções vazias para registros e erros.

O exemplo a seguir mostra um dispositivo registrado com êxito no gerenciamento de atualizações de recursos pelo serviço.

### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/983f03cd-03cd-983f-cd03-3f98cd033f98
```

### <a name="response"></a>Resposta
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
    "id": "983f03cd-03cd-983f-cd03-3f98cd033f98",
    "errors": [],
    "enrollments": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment",
        "updateCategory": "feature"
      }
    ]
  }
}
```

## <a name="unenroll-from-management-by-the-service-or-unregister-from-the-service"></a>Cancelar o registro do gerenciamento pelo serviço ou cancelar o registro do serviço 

Quando você cancela o registro de um dispositivo do gerenciamento pelo serviço para uma determinada categoria de atualização, o dispositivo não é mais gerenciado pelo serviço de implantação e pode começar a receber outras atualizações do Windows Update com base em sua configuração de política. Se o dispositivo for atribuído a qualquer implantação para a categoria de atualização fornecida, ele não receberá esse conteúdo. O dispositivo permanece registrado no serviço e ainda está registrado e recebendo conteúdo para outras categorias de atualização (se aplicável).

### <a name="request"></a>Solicitação

``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/unenrollAssets
Content-Type: application/json

{
  "updateCategory": "feature",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```

### <a name="response"></a>Resposta

``` http
HTTP/1.1 202 Accepted
```

Você pode cancelar o registro de um dispositivo do serviço completamente excluindo o objeto do dispositivo. Quando um dispositivo é cancelado, ele é cancelado automaticamente do gerenciamento pelo serviço para todas as categorias de atualização e removido de cada [deploymentAudience](/graph/api/resources/windowsupdates-deploymentaudience) e [updatableAssetGroup](/graph/api/resources/windowsupdates-updatableassetgroup).

### <a name="request"></a>Solicitação

``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{azureADDeviceId}
```

### <a name="response"></a>Resposta
``` http
HTTP/1.1 202 Accepted
```

