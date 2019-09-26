---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc31faba4c73616673a2e9f9203d37e21a7afc7a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191593"
---
# <a name="assign-action"></a><span data-ttu-id="7d73f-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="7d73f-103">assign action</span></span>

> <span data-ttu-id="7d73f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7d73f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d73f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d73f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d73f-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7d73f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d73f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d73f-107">Prerequisites</span></span>
<span data-ttu-id="7d73f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d73f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d73f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d73f-110">Permission type</span></span>|<span data-ttu-id="7d73f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d73f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d73f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d73f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d73f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d73f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7d73f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d73f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d73f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d73f-115">Not supported.</span></span>|
|<span data-ttu-id="7d73f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d73f-116">Application</span></span>|<span data-ttu-id="7d73f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d73f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d73f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d73f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="7d73f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d73f-119">Request headers</span></span>
|<span data-ttu-id="7d73f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d73f-120">Header</span></span>|<span data-ttu-id="7d73f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7d73f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d73f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d73f-122">Authorization</span></span>|<span data-ttu-id="7d73f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d73f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d73f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d73f-124">Accept</span></span>|<span data-ttu-id="7d73f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7d73f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d73f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d73f-126">Request body</span></span>
<span data-ttu-id="7d73f-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7d73f-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7d73f-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="7d73f-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7d73f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d73f-129">Property</span></span>|<span data-ttu-id="7d73f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d73f-130">Type</span></span>|<span data-ttu-id="7d73f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d73f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d73f-132">assignments</span><span class="sxs-lookup"><span data-stu-id="7d73f-132">assignments</span></span>|<span data-ttu-id="7d73f-133">Conjunto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7d73f-133">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="7d73f-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7d73f-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7d73f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d73f-135">Response</span></span>
<span data-ttu-id="7d73f-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7d73f-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7d73f-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d73f-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d73f-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d73f-138">Request</span></span>
<span data-ttu-id="7d73f-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d73f-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign

Content-type: application/json
Content-length: 351

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="7d73f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d73f-140">Response</span></span>
<span data-ttu-id="7d73f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d73f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




