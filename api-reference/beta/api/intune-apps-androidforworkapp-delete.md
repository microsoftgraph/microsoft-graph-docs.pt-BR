---
title: Excluir androidForWorkApp
description: Exclui androidForWorkApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eb496d60216e2521ab9dca28cbf76e3cfa46c22f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952447"
---
# <a name="delete-androidforworkapp"></a><span data-ttu-id="bc2ae-103">Excluir androidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="bc2ae-103">Delete androidForWorkApp</span></span>

> <span data-ttu-id="bc2ae-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc2ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc2ae-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc2ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc2ae-106">Exclui [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc2ae-106">Deletes a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc2ae-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc2ae-107">Prerequisites</span></span>
<span data-ttu-id="bc2ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc2ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc2ae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc2ae-110">Permission type</span></span>|<span data-ttu-id="bc2ae-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bc2ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc2ae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc2ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bc2ae-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc2ae-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bc2ae-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc2ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc2ae-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc2ae-115">Not supported.</span></span>|
|<span data-ttu-id="bc2ae-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc2ae-116">Application</span></span>|<span data-ttu-id="bc2ae-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc2ae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc2ae-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc2ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="bc2ae-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc2ae-119">Request headers</span></span>
|<span data-ttu-id="bc2ae-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc2ae-120">Header</span></span>|<span data-ttu-id="bc2ae-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bc2ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc2ae-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc2ae-122">Authorization</span></span>|<span data-ttu-id="bc2ae-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc2ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc2ae-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc2ae-124">Accept</span></span>|<span data-ttu-id="bc2ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bc2ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc2ae-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc2ae-126">Request body</span></span>
<span data-ttu-id="bc2ae-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc2ae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc2ae-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc2ae-128">Response</span></span>
<span data-ttu-id="bc2ae-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bc2ae-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bc2ae-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc2ae-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc2ae-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc2ae-131">Request</span></span>
<span data-ttu-id="bc2ae-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc2ae-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="bc2ae-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc2ae-133">Response</span></span>
<span data-ttu-id="bc2ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc2ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





