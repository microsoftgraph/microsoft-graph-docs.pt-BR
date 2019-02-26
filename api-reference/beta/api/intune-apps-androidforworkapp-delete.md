---
title: Excluir androidForWorkApp
description: Exclui androidForWorkApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa748ab86d9c1a9016edfbc2ef7aa332e3ae4f17
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169829"
---
# <a name="delete-androidforworkapp"></a><span data-ttu-id="3264e-103">Excluir androidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="3264e-103">Delete androidForWorkApp</span></span>

> <span data-ttu-id="3264e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3264e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3264e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3264e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3264e-106">Exclui [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span><span class="sxs-lookup"><span data-stu-id="3264e-106">Deletes a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3264e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3264e-107">Prerequisites</span></span>
<span data-ttu-id="3264e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3264e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3264e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3264e-110">Permission type</span></span>|<span data-ttu-id="3264e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3264e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3264e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3264e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3264e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3264e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3264e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3264e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3264e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3264e-115">Not supported.</span></span>|
|<span data-ttu-id="3264e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3264e-116">Application</span></span>|<span data-ttu-id="3264e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3264e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3264e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3264e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="3264e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3264e-119">Request headers</span></span>
|<span data-ttu-id="3264e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3264e-120">Header</span></span>|<span data-ttu-id="3264e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3264e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3264e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3264e-122">Authorization</span></span>|<span data-ttu-id="3264e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3264e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3264e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3264e-124">Accept</span></span>|<span data-ttu-id="3264e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3264e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3264e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3264e-126">Request body</span></span>
<span data-ttu-id="3264e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3264e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3264e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3264e-128">Response</span></span>
<span data-ttu-id="3264e-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3264e-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3264e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3264e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3264e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3264e-131">Request</span></span>
<span data-ttu-id="3264e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3264e-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="3264e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3264e-133">Response</span></span>
<span data-ttu-id="3264e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3264e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




