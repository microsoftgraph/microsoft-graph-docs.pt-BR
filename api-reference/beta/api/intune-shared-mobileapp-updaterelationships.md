---
title: ação updateRelationships
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ab0ffda284b455926d7f0bad3d17ecdb4b58de0
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537969"
---
# <a name="updaterelationships-action"></a><span data-ttu-id="42684-103">ação updateRelationships</span><span class="sxs-lookup"><span data-stu-id="42684-103">updateRelationships action</span></span>

> <span data-ttu-id="42684-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42684-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42684-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42684-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42684-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="42684-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42684-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42684-107">Prerequisites</span></span>
<span data-ttu-id="42684-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42684-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42684-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42684-110">Permission type</span></span>|<span data-ttu-id="42684-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42684-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42684-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42684-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="42684-113">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="42684-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="42684-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42684-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="42684-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42684-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42684-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42684-116">Not supported.</span></span>|
|<span data-ttu-id="42684-117">Application</span><span class="sxs-lookup"><span data-stu-id="42684-117">Application</span></span>||
| <span data-ttu-id="42684-118">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="42684-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="42684-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42684-119">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42684-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42684-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/updateRelationships
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/updateRelationships
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/updateRelationships
```

## <a name="request-headers"></a><span data-ttu-id="42684-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42684-121">Request headers</span></span>
|<span data-ttu-id="42684-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42684-122">Header</span></span>|<span data-ttu-id="42684-123">Valor</span><span class="sxs-lookup"><span data-stu-id="42684-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42684-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="42684-124">Authorization</span></span>|<span data-ttu-id="42684-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42684-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42684-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42684-126">Accept</span></span>|<span data-ttu-id="42684-127">application/json</span><span class="sxs-lookup"><span data-stu-id="42684-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42684-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42684-128">Request body</span></span>
<span data-ttu-id="42684-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="42684-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="42684-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="42684-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="42684-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42684-131">Property</span></span>|<span data-ttu-id="42684-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="42684-132">Type</span></span>|<span data-ttu-id="42684-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="42684-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42684-134">relações</span><span class="sxs-lookup"><span data-stu-id="42684-134">relationships</span></span>|<span data-ttu-id="42684-135">coleção [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="42684-135">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="42684-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="42684-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="42684-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="42684-137">Response</span></span>
<span data-ttu-id="42684-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="42684-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="42684-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42684-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="42684-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42684-140">Request</span></span>
<span data-ttu-id="42684-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42684-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="42684-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="42684-142">Response</span></span>
<span data-ttu-id="42684-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42684-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






