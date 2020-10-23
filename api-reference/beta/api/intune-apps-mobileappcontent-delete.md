---
title: Excluir mobileAppContent
description: Exclui mobileAppContent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a9ea278e6689a3f032781d531a046c01dd2a75c5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707567"
---
# <a name="delete-mobileappcontent"></a><span data-ttu-id="535e2-103">Excluir mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="535e2-103">Delete mobileAppContent</span></span>

<span data-ttu-id="535e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="535e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="535e2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="535e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="535e2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="535e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="535e2-107">Exclui [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="535e2-107">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="535e2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="535e2-108">Prerequisites</span></span>
<span data-ttu-id="535e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="535e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="535e2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="535e2-111">Permission type</span></span>|<span data-ttu-id="535e2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="535e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="535e2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="535e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="535e2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="535e2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="535e2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="535e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="535e2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="535e2-116">Not supported.</span></span>|
|<span data-ttu-id="535e2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="535e2-117">Application</span></span>|<span data-ttu-id="535e2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="535e2-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="535e2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="535e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="535e2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="535e2-120">Request headers</span></span>
|<span data-ttu-id="535e2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="535e2-121">Header</span></span>|<span data-ttu-id="535e2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="535e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="535e2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="535e2-123">Authorization</span></span>|<span data-ttu-id="535e2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="535e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="535e2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="535e2-125">Accept</span></span>|<span data-ttu-id="535e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="535e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="535e2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="535e2-127">Request body</span></span>
<span data-ttu-id="535e2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="535e2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="535e2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="535e2-129">Response</span></span>
<span data-ttu-id="535e2-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="535e2-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="535e2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="535e2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="535e2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="535e2-132">Request</span></span>
<span data-ttu-id="535e2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="535e2-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="535e2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="535e2-134">Response</span></span>
<span data-ttu-id="535e2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="535e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





