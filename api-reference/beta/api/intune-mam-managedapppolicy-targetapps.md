---
title: Ação targetApps
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 41746d8aab8694b7c4822b51abc80d68ef450ec0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36354160"
---
# <a name="targetapps-action"></a><span data-ttu-id="fb2da-103">ação targetApps</span><span class="sxs-lookup"><span data-stu-id="fb2da-103">targetApps action</span></span>

> <span data-ttu-id="fb2da-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fb2da-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb2da-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb2da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb2da-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fb2da-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb2da-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb2da-107">Prerequisites</span></span>
<span data-ttu-id="fb2da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb2da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb2da-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb2da-110">Permission type</span></span>|<span data-ttu-id="fb2da-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb2da-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb2da-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb2da-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fb2da-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb2da-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fb2da-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb2da-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb2da-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb2da-115">Not supported.</span></span>|
|<span data-ttu-id="fb2da-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb2da-116">Application</span></span>|<span data-ttu-id="fb2da-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb2da-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb2da-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb2da-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="fb2da-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb2da-119">Request headers</span></span>
|<span data-ttu-id="fb2da-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb2da-120">Header</span></span>|<span data-ttu-id="fb2da-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fb2da-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb2da-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb2da-122">Authorization</span></span>|<span data-ttu-id="fb2da-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb2da-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb2da-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb2da-124">Accept</span></span>|<span data-ttu-id="fb2da-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb2da-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb2da-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb2da-126">Request body</span></span>
<span data-ttu-id="fb2da-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="fb2da-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fb2da-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="fb2da-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fb2da-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb2da-129">Property</span></span>|<span data-ttu-id="fb2da-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb2da-130">Type</span></span>|<span data-ttu-id="fb2da-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb2da-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb2da-132">apps</span><span class="sxs-lookup"><span data-stu-id="fb2da-132">apps</span></span>|<span data-ttu-id="fb2da-133">Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb2da-133">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="fb2da-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fb2da-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fb2da-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb2da-135">Response</span></span>
<span data-ttu-id="fb2da-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fb2da-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fb2da-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb2da-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb2da-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb2da-138">Request</span></span>
<span data-ttu-id="fb2da-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb2da-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="fb2da-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb2da-140">Response</span></span>
<span data-ttu-id="fb2da-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb2da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






