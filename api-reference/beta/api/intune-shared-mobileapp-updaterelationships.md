---
title: ação updateRelationships
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d9626895c7df4a8e8ccac0bc999752c797b9e0b7
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199387"
---
# <a name="updaterelationships-action"></a><span data-ttu-id="d11ae-103">ação updateRelationships</span><span class="sxs-lookup"><span data-stu-id="d11ae-103">updateRelationships action</span></span>

> <span data-ttu-id="d11ae-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d11ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d11ae-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d11ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d11ae-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d11ae-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d11ae-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d11ae-107">Prerequisites</span></span>
<span data-ttu-id="d11ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d11ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d11ae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d11ae-110">Permission type</span></span>|<span data-ttu-id="d11ae-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d11ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d11ae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d11ae-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d11ae-113">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="d11ae-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d11ae-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d11ae-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d11ae-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d11ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d11ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d11ae-116">Not supported.</span></span>|
|<span data-ttu-id="d11ae-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d11ae-117">Application</span></span>||
| <span data-ttu-id="d11ae-118">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="d11ae-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d11ae-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d11ae-119">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d11ae-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d11ae-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/updateRelationships
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/updateRelationships
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/updateRelationships
```

## <a name="request-headers"></a><span data-ttu-id="d11ae-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d11ae-121">Request headers</span></span>
|<span data-ttu-id="d11ae-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d11ae-122">Header</span></span>|<span data-ttu-id="d11ae-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d11ae-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d11ae-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d11ae-124">Authorization</span></span>|<span data-ttu-id="d11ae-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d11ae-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d11ae-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d11ae-126">Accept</span></span>|<span data-ttu-id="d11ae-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d11ae-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d11ae-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d11ae-128">Request body</span></span>
<span data-ttu-id="d11ae-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d11ae-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d11ae-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d11ae-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d11ae-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d11ae-131">Property</span></span>|<span data-ttu-id="d11ae-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d11ae-132">Type</span></span>|<span data-ttu-id="d11ae-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d11ae-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d11ae-134">relações</span><span class="sxs-lookup"><span data-stu-id="d11ae-134">relationships</span></span>|<span data-ttu-id="d11ae-135">coleção [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d11ae-135">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="d11ae-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d11ae-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d11ae-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d11ae-137">Response</span></span>
<span data-ttu-id="d11ae-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d11ae-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d11ae-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d11ae-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="d11ae-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d11ae-140">Request</span></span>
<span data-ttu-id="d11ae-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d11ae-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/updateRelationships

Content-type: application/json
Content-length: 256

{
  "relationships": [
    {
      "@odata.type": "#microsoft.graph.mobileAppRelationship",
      "id": "7b4b5b14-5b14-7b4b-145b-4b7b145b4b7b",
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d11ae-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d11ae-142">Response</span></span>
<span data-ttu-id="d11ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d11ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




