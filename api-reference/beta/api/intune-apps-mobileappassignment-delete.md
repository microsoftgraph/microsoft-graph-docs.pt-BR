---
title: Excluir mobileAppAssignment
description: Exclui mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86bb59b327278c50fa7cdcd79e4da8d3d8ce1fbb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43404686"
---
# <a name="delete-mobileappassignment"></a><span data-ttu-id="3bc71-103">Excluir mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="3bc71-103">Delete mobileAppAssignment</span></span>

<span data-ttu-id="3bc71-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bc71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3bc71-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3bc71-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bc71-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3bc71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bc71-107">Exclui [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3bc71-107">Deletes a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bc71-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3bc71-108">Prerequisites</span></span>
<span data-ttu-id="3bc71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bc71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bc71-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3bc71-111">Permission type</span></span>|<span data-ttu-id="3bc71-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3bc71-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bc71-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3bc71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3bc71-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bc71-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3bc71-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3bc71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bc71-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bc71-116">Not supported.</span></span>|
|<span data-ttu-id="3bc71-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3bc71-117">Application</span></span>|<span data-ttu-id="3bc71-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bc71-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bc71-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3bc71-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3bc71-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3bc71-120">Request headers</span></span>
|<span data-ttu-id="3bc71-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3bc71-121">Header</span></span>|<span data-ttu-id="3bc71-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3bc71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bc71-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3bc71-123">Authorization</span></span>|<span data-ttu-id="3bc71-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3bc71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bc71-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3bc71-125">Accept</span></span>|<span data-ttu-id="3bc71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3bc71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bc71-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3bc71-127">Request body</span></span>
<span data-ttu-id="3bc71-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3bc71-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bc71-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bc71-129">Response</span></span>
<span data-ttu-id="3bc71-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3bc71-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3bc71-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3bc71-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bc71-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bc71-132">Request</span></span>
<span data-ttu-id="3bc71-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3bc71-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="3bc71-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bc71-134">Response</span></span>
<span data-ttu-id="3bc71-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3bc71-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



