---
title: Excluir microsoftStoreForBusinessApp
description: Exclui microsoftStoreForBusinessApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 55da404c8375958b1c09dd18d57acc52c436b86e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974381"
---
# <a name="delete-microsoftstoreforbusinessapp"></a><span data-ttu-id="b0cee-103">Excluir microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="b0cee-103">Delete microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="b0cee-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0cee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0cee-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0cee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0cee-106">Exclui [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0cee-106">Deletes a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0cee-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0cee-107">Prerequisites</span></span>
<span data-ttu-id="b0cee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0cee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0cee-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0cee-110">Permission type</span></span>|<span data-ttu-id="b0cee-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0cee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0cee-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0cee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0cee-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0cee-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b0cee-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0cee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0cee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0cee-115">Not supported.</span></span>|
|<span data-ttu-id="b0cee-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0cee-116">Application</span></span>|<span data-ttu-id="b0cee-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0cee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0cee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0cee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="b0cee-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0cee-119">Request headers</span></span>
|<span data-ttu-id="b0cee-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0cee-120">Header</span></span>|<span data-ttu-id="b0cee-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b0cee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0cee-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0cee-122">Authorization</span></span>|<span data-ttu-id="b0cee-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0cee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0cee-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b0cee-124">Accept</span></span>|<span data-ttu-id="b0cee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b0cee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0cee-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0cee-126">Request body</span></span>
<span data-ttu-id="b0cee-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b0cee-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0cee-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0cee-128">Response</span></span>
<span data-ttu-id="b0cee-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b0cee-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b0cee-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0cee-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0cee-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0cee-131">Request</span></span>
<span data-ttu-id="b0cee-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0cee-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="b0cee-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0cee-133">Response</span></span>
<span data-ttu-id="b0cee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0cee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





