---
title: Excluir iosVppAppAssignedUserLicense
description: Exclui iosVppAppAssignedUserLicense.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b9585e3a6cfc6a5af2df7ddce0b03cd7c2e95f3d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958477"
---
# <a name="delete-iosvppappassigneduserlicense"></a><span data-ttu-id="e4481-103">Excluir iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="e4481-103">Delete iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="e4481-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4481-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4481-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4481-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4481-106">Exclui [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span><span class="sxs-lookup"><span data-stu-id="e4481-106">Deletes a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4481-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4481-107">Prerequisites</span></span>
<span data-ttu-id="e4481-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4481-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4481-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4481-110">Permission type</span></span>|<span data-ttu-id="e4481-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4481-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4481-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4481-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4481-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4481-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e4481-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4481-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4481-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4481-115">Not supported.</span></span>|
|<span data-ttu-id="e4481-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4481-116">Application</span></span>|<span data-ttu-id="e4481-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4481-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4481-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4481-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="e4481-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4481-119">Request headers</span></span>
|<span data-ttu-id="e4481-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4481-120">Header</span></span>|<span data-ttu-id="e4481-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e4481-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4481-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4481-122">Authorization</span></span>|<span data-ttu-id="e4481-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4481-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4481-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e4481-124">Accept</span></span>|<span data-ttu-id="e4481-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4481-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4481-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4481-126">Request body</span></span>
<span data-ttu-id="e4481-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4481-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4481-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4481-128">Response</span></span>
<span data-ttu-id="e4481-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e4481-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e4481-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4481-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4481-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4481-131">Request</span></span>
<span data-ttu-id="e4481-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4481-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

### <a name="response"></a><span data-ttu-id="e4481-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4481-133">Response</span></span>
<span data-ttu-id="e4481-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4481-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




