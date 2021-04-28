---
title: Registrar-se no gerenciamento de atualizações pelo serviço de implantação Windows Atualização para Empresas
description: Quando um dispositivo é inscrito no gerenciamento de atualizações pelo serviço de implantação do Windows Update for Business, você pode usar o serviço de implantação para gerenciar o conteúdo fornecido do Windows Update para esse dispositivo.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 2492a447aa26bbc3de6835a76c5876e55cac774c
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067657"
---
# <a name="enroll-in-update-management-by-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="97b3e-103">Registrar-se no gerenciamento de atualizações pelo serviço de implantação Windows Atualização para Empresas</span><span class="sxs-lookup"><span data-stu-id="97b3e-103">Enroll in update management by the Windows Update for Business deployment service</span></span>

<span data-ttu-id="97b3e-104">Ao registrar o dispositivo no gerenciamento de atualização pelo serviço de implantação do Windows Update for Business, você pode usar o serviço de implantação para gerenciar o conteúdo fornecido do Windows Update para esse dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97b3e-104">When you enroll device in update management by the Windows Update for Business deployment service, you can use the deployment service to manage content delivered from Windows Update to that device.</span></span> <span data-ttu-id="97b3e-105">Você pode registrar um dispositivo no gerenciamento de atualizações por categoria de atualização.</span><span class="sxs-lookup"><span data-stu-id="97b3e-105">You can enroll a device in update management by update category.</span></span>

<span data-ttu-id="97b3e-106">Hoje, o serviço de implantação dá suporte ao registro no gerenciamento de Windows 10 de recursos.</span><span class="sxs-lookup"><span data-stu-id="97b3e-106">Today, the deployment service supports enrollment in management of Windows 10 feature updates.</span></span> <span data-ttu-id="97b3e-107">Neste momento, o serviço de implantação não exige registro no gerenciamento de atualizações de qualidade Windows 10 para implantar atualizações de qualidade aceleradas.</span><span class="sxs-lookup"><span data-stu-id="97b3e-107">At this time, the deployment service does not require enrollment in management of Windows 10 quality updates in order to deploy expedited quality updates.</span></span>

## <a name="enroll-the-device-in-update-management"></a><span data-ttu-id="97b3e-108">Registrar o dispositivo no gerenciamento de atualizações</span><span class="sxs-lookup"><span data-stu-id="97b3e-108">Enroll the device in update management</span></span>

<span data-ttu-id="97b3e-109">Quando você registra um dispositivo no gerenciamento de uma determinada categoria de atualização, o serviço de implantação se torna a autoridade para atualizações dessa categoria provenientes do Windows Update.</span><span class="sxs-lookup"><span data-stu-id="97b3e-109">When you enroll a device in management for a certain update category, the deployment service becomes the authority for updates of that category coming from Windows Update.</span></span> <span data-ttu-id="97b3e-110">Como resultado, os dispositivos não recebem atualizações dessa categoria do Windows Update até que você implante uma atualização usando o serviço de implantação atribuindo-a a uma [implantação](windowsupdates-deployments.md).</span><span class="sxs-lookup"><span data-stu-id="97b3e-110">As a result, devices do not receive updates of that category from Windows Update until you deploy an update using the deployment service by assigning it to a [deployment](windowsupdates-deployments.md).</span></span> <span data-ttu-id="97b3e-111">Os dispositivos são registrados automaticamente com o serviço quando registrados no gerenciamento pelo serviço (ou seja, um [objeto azureADDevice](/graph/api/resources/windowsupdates-azureaddevice.md) é criado automaticamente se ainda não existir).</span><span class="sxs-lookup"><span data-stu-id="97b3e-111">Devices are automatically registered with the service when enrolled in management by the service (i.e. an [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice.md) object is automatically created if it does not already exist).</span></span>

### <a name="request"></a><span data-ttu-id="97b3e-112">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97b3e-112">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="97b3e-113">Resposta</span><span class="sxs-lookup"><span data-stu-id="97b3e-113">Response</span></span>

``` http
HTTP/1.1 202 Accepted
```

## <a name="check-the-enrollment-state-of-a-device"></a><span data-ttu-id="97b3e-114">Verificar o estado de registro de um dispositivo</span><span class="sxs-lookup"><span data-stu-id="97b3e-114">Check the enrollment state of a device</span></span>

<span data-ttu-id="97b3e-115">Você pode verificar o estado [](/graph/api/windowsupdates-azureaddevice-get) de registro de um dispositivo  ao obter o dispositivo e ver as propriedades **de** registro e erros no **objeto azureADDevice.**</span><span class="sxs-lookup"><span data-stu-id="97b3e-115">You can check the enrollment state of a device by [getting the device](/graph/api/windowsupdates-azureaddevice-get) and looking at the **enrollments** and **errors** properties on the **azureADDevice** object.</span></span> <span data-ttu-id="97b3e-116">Um dispositivo que é inscrito com êxito no gerenciamento de atualizações tem um [objeto updateManagementEnrollment](/graph/api/resources/windowsupdates-updatemanagementenrollment) na coleção enrollments e não tem nenhum objeto [updateableAssetError](/graph/api/resources/windowsupdates-updatableasseterror) na coleção errors.</span><span class="sxs-lookup"><span data-stu-id="97b3e-116">A device that is successfully enrolled in update management has an [updateManagementEnrollment](/graph/api/resources/windowsupdates-updatemanagementenrollment) object in the enrollments collection, and it does not have any [updatableAssetError](/graph/api/resources/windowsupdates-updatableasseterror) objects in the errors collection.</span></span> <span data-ttu-id="97b3e-117">Um dispositivo que o serviço tentou registrar, mas encontrou um erro preencheu coleções para registro e erros.</span><span class="sxs-lookup"><span data-stu-id="97b3e-117">A device that the service tried to enroll but encountered an error has populated collections for both enrollments and errors.</span></span> <span data-ttu-id="97b3e-118">Um dispositivo para o qual o serviço não recebeu solicitações de registro tem coleções vazias para registro e erros.</span><span class="sxs-lookup"><span data-stu-id="97b3e-118">A device for which the service has not received any enrollment requests has empty collections for both enrollments and errors.</span></span>

<span data-ttu-id="97b3e-119">O exemplo a seguir mostra um dispositivo que é inscrito com êxito no gerenciamento de atualizações de recursos pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="97b3e-119">The following example shows a device that is successfully enrolled in management of feature updates by the service.</span></span>

### <a name="request"></a><span data-ttu-id="97b3e-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97b3e-120">Request</span></span>

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/983f03cd-03cd-983f-cd03-3f98cd033f98
```

### <a name="response"></a><span data-ttu-id="97b3e-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="97b3e-121">Response</span></span>
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

## <a name="unenroll-from-management-by-the-service-or-unregister-from-the-service"></a><span data-ttu-id="97b3e-122">Desemitir do gerenciamento pelo serviço ou não registro no serviço</span><span class="sxs-lookup"><span data-stu-id="97b3e-122">Unenroll from management by the service or unregister from the service</span></span> 

<span data-ttu-id="97b3e-123">Quando você desemarro um dispositivo do gerenciamento pelo serviço para uma determinada categoria de atualização, o dispositivo não é mais gerenciado pelo serviço de implantação e pode começar a receber outras atualizações do Windows Update com base em sua configuração de política.</span><span class="sxs-lookup"><span data-stu-id="97b3e-123">When you unenroll a device from management by the service for a given update category, the device is no longer managed by the deployment service and may start receiving other updates from Windows Update based on its policy configuration.</span></span> <span data-ttu-id="97b3e-124">Se o dispositivo for atribuído a qualquer implantação para a categoria de atualização determinada, ele não receberá esse conteúdo.</span><span class="sxs-lookup"><span data-stu-id="97b3e-124">If the device is assigned to any deployments for the given update category, it does not receive that content.</span></span> <span data-ttu-id="97b3e-125">O dispositivo permanece registrado no serviço e ainda está registrado e recebendo conteúdo para outras categorias de atualização (se aplicável).</span><span class="sxs-lookup"><span data-stu-id="97b3e-125">The device remains registered with the service and is still enrolled and receiving content for other update categories (if applicable).</span></span>

### <a name="request"></a><span data-ttu-id="97b3e-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97b3e-126">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="97b3e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="97b3e-127">Response</span></span>

``` http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="97b3e-128">Você pode desatar um dispositivo do serviço completamente excluindo o objeto device.</span><span class="sxs-lookup"><span data-stu-id="97b3e-128">You can unregister a device from the service completely by deleting the device object.</span></span> <span data-ttu-id="97b3e-129">Quando um dispositivo é sem registro, ele é automaticamente desinteressado do gerenciamento pelo serviço para todas as categorias de atualização e removido de todos os públicos de implantação e [grupos updateableAsset.](/graph/api/resources/windowsupdates-updatableasset)</span><span class="sxs-lookup"><span data-stu-id="97b3e-129">When a device is unregistered, it is automatically unenrolled from management by the service for all update categories and removed from all deployment audiences and [updatableAsset](/graph/api/resources/windowsupdates-updatableasset) groups.</span></span>

### <a name="request"></a><span data-ttu-id="97b3e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97b3e-130">Request</span></span>

``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{azureADDeviceId}
```

### <a name="response"></a><span data-ttu-id="97b3e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="97b3e-131">Response</span></span>
``` http
HTTP/1.1 202 Accepted
```

