---
title: ação updateRelationships
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4668438f40570d160f25916a0338432f45c6fedb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022397"
---
# <a name="updaterelationships-action"></a><span data-ttu-id="97266-103">ação updateRelationships</span><span class="sxs-lookup"><span data-stu-id="97266-103">updateRelationships action</span></span>

<span data-ttu-id="97266-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97266-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97266-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97266-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97266-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97266-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97266-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="97266-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97266-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97266-108">Prerequisites</span></span>
<span data-ttu-id="97266-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97266-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97266-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97266-111">Permission type</span></span>|<span data-ttu-id="97266-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97266-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97266-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97266-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="97266-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="97266-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="97266-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97266-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="97266-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97266-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97266-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97266-117">Not supported.</span></span>|
|<span data-ttu-id="97266-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97266-118">Application</span></span>||
| <span data-ttu-id="97266-119">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="97266-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="97266-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97266-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97266-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97266-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/updateRelationships
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/updateRelationships
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/updateRelationships
```

## <a name="request-headers"></a><span data-ttu-id="97266-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97266-122">Request headers</span></span>
|<span data-ttu-id="97266-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97266-123">Header</span></span>|<span data-ttu-id="97266-124">Valor</span><span class="sxs-lookup"><span data-stu-id="97266-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97266-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="97266-125">Authorization</span></span>|<span data-ttu-id="97266-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97266-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97266-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97266-127">Accept</span></span>|<span data-ttu-id="97266-128">application/json</span><span class="sxs-lookup"><span data-stu-id="97266-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97266-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97266-129">Request body</span></span>
<span data-ttu-id="97266-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="97266-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="97266-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="97266-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="97266-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97266-132">Property</span></span>|<span data-ttu-id="97266-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="97266-133">Type</span></span>|<span data-ttu-id="97266-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="97266-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97266-135">relações</span><span class="sxs-lookup"><span data-stu-id="97266-135">relationships</span></span>|<span data-ttu-id="97266-136">coleção [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="97266-136">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="97266-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="97266-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="97266-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="97266-138">Response</span></span>
<span data-ttu-id="97266-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="97266-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="97266-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97266-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="97266-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97266-141">Request</span></span>
<span data-ttu-id="97266-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97266-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="97266-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="97266-143">Response</span></span>
<span data-ttu-id="97266-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97266-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









