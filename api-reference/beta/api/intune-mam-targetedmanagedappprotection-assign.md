---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 593dc93879aed733738a80eece8a9a2105c59e1c
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178336"
---
# <a name="assign-action"></a><span data-ttu-id="14808-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="14808-103">assign action</span></span>

<span data-ttu-id="14808-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14808-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14808-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14808-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14808-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14808-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14808-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="14808-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14808-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14808-108">Prerequisites</span></span>
<span data-ttu-id="14808-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14808-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14808-111">Permission type</span></span>|<span data-ttu-id="14808-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14808-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14808-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14808-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14808-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14808-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="14808-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14808-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14808-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14808-116">Not supported.</span></span>|
|<span data-ttu-id="14808-117">Application</span><span class="sxs-lookup"><span data-stu-id="14808-117">Application</span></span>|<span data-ttu-id="14808-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14808-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14808-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14808-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="14808-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14808-120">Request headers</span></span>
|<span data-ttu-id="14808-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14808-121">Header</span></span>|<span data-ttu-id="14808-122">Valor</span><span class="sxs-lookup"><span data-stu-id="14808-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14808-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="14808-123">Authorization</span></span>|<span data-ttu-id="14808-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14808-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14808-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="14808-125">Accept</span></span>|<span data-ttu-id="14808-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14808-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14808-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14808-127">Request body</span></span>
<span data-ttu-id="14808-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="14808-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="14808-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="14808-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="14808-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14808-130">Property</span></span>|<span data-ttu-id="14808-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="14808-131">Type</span></span>|<span data-ttu-id="14808-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="14808-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14808-133">assignments</span><span class="sxs-lookup"><span data-stu-id="14808-133">assignments</span></span>|<span data-ttu-id="14808-134">Conjunto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="14808-134">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="14808-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="14808-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="14808-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="14808-136">Response</span></span>
<span data-ttu-id="14808-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="14808-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="14808-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14808-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="14808-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14808-139">Request</span></span>
<span data-ttu-id="14808-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14808-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign

Content-type: application/json
Content-length: 339

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="14808-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="14808-141">Response</span></span>
<span data-ttu-id="14808-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14808-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



