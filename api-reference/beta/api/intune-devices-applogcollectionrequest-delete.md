---
title: Excluir appLogCollectionRequest
description: Exclui appLogCollectionRequest.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12a8c59a5ec7434afadcb044bd158443ceb7e886
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959324"
---
# <a name="delete-applogcollectionrequest"></a><span data-ttu-id="fee46-103">Excluir appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="fee46-103">Delete appLogCollectionRequest</span></span>

> <span data-ttu-id="fee46-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fee46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fee46-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fee46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fee46-106">Exclui [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span><span class="sxs-lookup"><span data-stu-id="fee46-106">Deletes a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fee46-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fee46-107">Prerequisites</span></span>
<span data-ttu-id="fee46-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fee46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fee46-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fee46-110">Permission type</span></span>|<span data-ttu-id="fee46-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fee46-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fee46-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fee46-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fee46-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fee46-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fee46-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fee46-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fee46-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fee46-115">Not supported.</span></span>|
|<span data-ttu-id="fee46-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fee46-116">Application</span></span>|<span data-ttu-id="fee46-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fee46-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fee46-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fee46-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="fee46-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fee46-119">Request headers</span></span>
|<span data-ttu-id="fee46-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fee46-120">Header</span></span>|<span data-ttu-id="fee46-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fee46-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fee46-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fee46-122">Authorization</span></span>|<span data-ttu-id="fee46-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fee46-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fee46-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fee46-124">Accept</span></span>|<span data-ttu-id="fee46-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fee46-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fee46-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fee46-126">Request body</span></span>
<span data-ttu-id="fee46-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fee46-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fee46-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fee46-128">Response</span></span>
<span data-ttu-id="fee46-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fee46-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fee46-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fee46-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fee46-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fee46-131">Request</span></span>
<span data-ttu-id="fee46-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fee46-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

### <a name="response"></a><span data-ttu-id="fee46-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fee46-133">Response</span></span>
<span data-ttu-id="fee46-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fee46-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





