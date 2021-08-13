---
title: Registrar-se no gerenciamento de atualizações pelo serviço de implantação Windows Atualização para Empresas
description: Quando um dispositivo é inscrito no gerenciamento de atualizações pelo serviço de implantação do Windows Update for Business, você pode usar o serviço de implantação para gerenciar o conteúdo fornecido do Windows Update para esse dispositivo.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 7e20fd175e1dc70c843a39ea8b0b818f45d975f1aa63d92ad3374ebc1ac961ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54225640"
---
# <a name="enroll-in-update-management-by-the-windows-update-for-business-deployment-service"></a>Registrar-se no gerenciamento de atualizações pelo serviço de implantação Windows Atualização para Empresas

Ao registrar o dispositivo no gerenciamento de atualização pelo serviço de implantação do Windows Update for Business, você pode usar o serviço de implantação para gerenciar o conteúdo fornecido do Windows Update para esse dispositivo. Você pode registrar um dispositivo no gerenciamento de atualizações por categoria de atualização.

Hoje, o serviço de implantação dá suporte ao registro no gerenciamento de Windows 10 de recursos. Neste momento, o serviço de implantação não exige registro no gerenciamento de atualizações de qualidade Windows 10 para implantar atualizações de qualidade aceleradas.

## <a name="enroll-the-device-in-update-management"></a>Registrar o dispositivo no gerenciamento de atualizações

Quando você registra um dispositivo no gerenciamento de uma determinada categoria de atualização, o serviço de implantação se torna a autoridade para atualizações dessa categoria provenientes do Windows Update. Como resultado, os dispositivos não recebem atualizações dessa categoria do Windows Update até que você implante uma atualização usando o serviço de implantação atribuindo-a a uma [implantação](windowsupdates-deployments.md). Os dispositivos são registrados automaticamente com o serviço quando registrados no gerenciamento pelo serviço (ou seja, um [objeto azureADDevice](/graph/api/resources/windowsupdates-azureaddevice.md) é criado automaticamente se ainda não existir).

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

Você pode verificar o estado [](/graph/api/windowsupdates-azureaddevice-get) de registro de um dispositivo  ao obter o dispositivo e ver as propriedades **de** registro e erros no **objeto azureADDevice.** Um dispositivo que é inscrito com êxito no gerenciamento de atualizações tem um [objeto updateManagementEnrollment](/graph/api/resources/windowsupdates-updatemanagementenrollment) na coleção enrollments e não tem nenhum objeto [updateableAssetError](/graph/api/resources/windowsupdates-updatableasseterror) na coleção errors. Um dispositivo que o serviço tentou registrar, mas encontrou um erro preencheu coleções para registro e erros. Um dispositivo para o qual o serviço não recebeu solicitações de registro tem coleções vazias para registro e erros.

O exemplo a seguir mostra um dispositivo que é inscrito com êxito no gerenciamento de atualizações de recursos pelo serviço.

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

## <a name="unenroll-from-management-by-the-service-or-unregister-from-the-service"></a>Desemitir do gerenciamento pelo serviço ou não registro no serviço 

Quando você desemarro um dispositivo do gerenciamento pelo serviço para uma determinada categoria de atualização, o dispositivo não é mais gerenciado pelo serviço de implantação e pode começar a receber outras atualizações do Windows Update com base em sua configuração de política. Se o dispositivo for atribuído a qualquer implantação para a categoria de atualização determinada, ele não receberá esse conteúdo. O dispositivo permanece registrado no serviço e ainda está registrado e recebendo conteúdo para outras categorias de atualização (se aplicável).

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

Você pode desatar um dispositivo do serviço completamente excluindo o objeto device. Quando um dispositivo é não registro, ele é automaticamente desinteressado do gerenciamento pelo serviço para todas as categorias de atualização e removido de todas as [implantaçõesAudiência](/graph/api/resources/windowsupdates-deploymentaudience) e [updateableAssetGroup](/graph/api/resources/windowsupdates-updatableassetgroup).

### <a name="request"></a>Solicitação

``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{azureADDeviceId}
```

### <a name="response"></a>Resposta
``` http
HTTP/1.1 202 Accepted
```

