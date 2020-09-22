---
title: Ação targetApps
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d68d46eb78c34a73acb4f0a9b0759c5fcddaacd8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079491"
---
# <a name="targetapps-action"></a><span data-ttu-id="d056c-103">ação targetApps</span><span class="sxs-lookup"><span data-stu-id="d056c-103">targetApps action</span></span>

<span data-ttu-id="d056c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d056c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d056c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d056c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d056c-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d056c-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d056c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d056c-107">Prerequisites</span></span>
<span data-ttu-id="d056c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d056c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d056c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d056c-110">Permission type</span></span>|<span data-ttu-id="d056c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d056c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d056c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d056c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d056c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d056c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d056c-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d056c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d056c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d056c-115">Not supported.</span></span>|
|<span data-ttu-id="d056c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d056c-116">Application</span></span>|<span data-ttu-id="d056c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d056c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d056c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d056c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="d056c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d056c-119">Request headers</span></span>
|<span data-ttu-id="d056c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d056c-120">Header</span></span>|<span data-ttu-id="d056c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d056c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d056c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d056c-122">Authorization</span></span>|<span data-ttu-id="d056c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d056c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d056c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d056c-124">Accept</span></span>|<span data-ttu-id="d056c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d056c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d056c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d056c-126">Request body</span></span>
<span data-ttu-id="d056c-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d056c-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d056c-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d056c-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d056c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d056c-129">Property</span></span>|<span data-ttu-id="d056c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d056c-130">Type</span></span>|<span data-ttu-id="d056c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d056c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d056c-132">apps</span><span class="sxs-lookup"><span data-stu-id="d056c-132">apps</span></span>|<span data-ttu-id="d056c-133">Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d056c-133">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="d056c-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d056c-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d056c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d056c-135">Response</span></span>
<span data-ttu-id="d056c-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d056c-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d056c-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d056c-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="d056c-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d056c-138">Request</span></span>
<span data-ttu-id="d056c-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d056c-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

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

### <a name="response"></a><span data-ttu-id="d056c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d056c-140">Response</span></span>
<span data-ttu-id="d056c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d056c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









