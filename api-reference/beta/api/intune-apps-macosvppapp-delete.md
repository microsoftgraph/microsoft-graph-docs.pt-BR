---
title: Excluir macOsVppApp
description: Exclui macOsVppApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 046d026d1593cc817daccd7f8879b8e6f0233c4a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43409929"
---
# <a name="delete-macosvppapp"></a><span data-ttu-id="ed97d-103">Excluir macOsVppApp</span><span class="sxs-lookup"><span data-stu-id="ed97d-103">Delete macOsVppApp</span></span>

<span data-ttu-id="ed97d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed97d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed97d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ed97d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed97d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed97d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed97d-107">Exclui [macOsVppApp](../resources/intune-apps-macosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="ed97d-107">Deletes a [macOsVppApp](../resources/intune-apps-macosvppapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed97d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed97d-108">Prerequisites</span></span>
<span data-ttu-id="ed97d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed97d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed97d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed97d-111">Permission type</span></span>|<span data-ttu-id="ed97d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed97d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed97d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed97d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed97d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed97d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ed97d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed97d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed97d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed97d-116">Not supported.</span></span>|
|<span data-ttu-id="ed97d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed97d-117">Application</span></span>|<span data-ttu-id="ed97d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed97d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed97d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed97d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="ed97d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed97d-120">Request headers</span></span>
|<span data-ttu-id="ed97d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed97d-121">Header</span></span>|<span data-ttu-id="ed97d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ed97d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed97d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed97d-123">Authorization</span></span>|<span data-ttu-id="ed97d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed97d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed97d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed97d-125">Accept</span></span>|<span data-ttu-id="ed97d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed97d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed97d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed97d-127">Request body</span></span>
<span data-ttu-id="ed97d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed97d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed97d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed97d-129">Response</span></span>
<span data-ttu-id="ed97d-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ed97d-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ed97d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed97d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed97d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed97d-132">Request</span></span>
<span data-ttu-id="ed97d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed97d-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="ed97d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed97d-134">Response</span></span>
<span data-ttu-id="ed97d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed97d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



