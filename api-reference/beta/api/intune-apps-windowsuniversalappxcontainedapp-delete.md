---
title: Excluir windowsUniversalAppXContainedApp
description: Exclui windowsUniversalAppXContainedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83aa21a36316ee43b00bae11a31ac196c6e10ffb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976001"
---
# <a name="delete-windowsuniversalappxcontainedapp"></a><span data-ttu-id="5bf88-103">Excluir windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="5bf88-103">Delete windowsUniversalAppXContainedApp</span></span>

<span data-ttu-id="5bf88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bf88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5bf88-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5bf88-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bf88-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5bf88-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bf88-107">Exclui [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bf88-107">Deletes a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bf88-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5bf88-108">Prerequisites</span></span>
<span data-ttu-id="5bf88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bf88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bf88-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bf88-111">Permission type</span></span>|<span data-ttu-id="5bf88-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5bf88-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bf88-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bf88-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5bf88-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bf88-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5bf88-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bf88-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bf88-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bf88-116">Not supported.</span></span>|
|<span data-ttu-id="5bf88-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bf88-117">Application</span></span>|<span data-ttu-id="5bf88-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bf88-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bf88-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bf88-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="5bf88-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5bf88-120">Request headers</span></span>
|<span data-ttu-id="5bf88-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5bf88-121">Header</span></span>|<span data-ttu-id="5bf88-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5bf88-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bf88-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bf88-123">Authorization</span></span>|<span data-ttu-id="5bf88-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bf88-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bf88-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5bf88-125">Accept</span></span>|<span data-ttu-id="5bf88-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5bf88-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bf88-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5bf88-127">Request body</span></span>
<span data-ttu-id="5bf88-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5bf88-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bf88-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bf88-129">Response</span></span>
<span data-ttu-id="5bf88-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5bf88-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5bf88-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5bf88-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bf88-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bf88-132">Request</span></span>
<span data-ttu-id="5bf88-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bf88-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
```

### <a name="response"></a><span data-ttu-id="5bf88-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bf88-134">Response</span></span>
<span data-ttu-id="5bf88-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5bf88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






