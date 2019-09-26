---
title: Excluir androidManagedStoreApp
description: Exclui androidManagedStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c928bc0580c39655288ea61a1798a2bdd43d4231
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173861"
---
# <a name="delete-androidmanagedstoreapp"></a><span data-ttu-id="41556-103">Excluir androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="41556-103">Delete androidManagedStoreApp</span></span>

> <span data-ttu-id="41556-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="41556-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41556-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41556-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41556-106">Exclui [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="41556-106">Deletes a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41556-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41556-107">Prerequisites</span></span>
<span data-ttu-id="41556-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41556-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41556-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41556-110">Permission type</span></span>|<span data-ttu-id="41556-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41556-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41556-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41556-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41556-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41556-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="41556-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41556-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41556-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41556-115">Not supported.</span></span>|
|<span data-ttu-id="41556-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41556-116">Application</span></span>|<span data-ttu-id="41556-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41556-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41556-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41556-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="41556-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41556-119">Request headers</span></span>
|<span data-ttu-id="41556-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41556-120">Header</span></span>|<span data-ttu-id="41556-121">Valor</span><span class="sxs-lookup"><span data-stu-id="41556-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41556-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="41556-122">Authorization</span></span>|<span data-ttu-id="41556-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41556-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41556-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41556-124">Accept</span></span>|<span data-ttu-id="41556-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41556-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41556-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41556-126">Request body</span></span>
<span data-ttu-id="41556-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41556-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41556-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="41556-128">Response</span></span>
<span data-ttu-id="41556-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="41556-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="41556-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41556-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="41556-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41556-131">Request</span></span>
<span data-ttu-id="41556-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41556-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="41556-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="41556-133">Response</span></span>
<span data-ttu-id="41556-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41556-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




