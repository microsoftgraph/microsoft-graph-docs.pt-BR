---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eed59b6fee36e77dc504efab3279cdb073244747
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458137"
---
# <a name="assign-action"></a><span data-ttu-id="892ce-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="892ce-103">assign action</span></span>

<span data-ttu-id="892ce-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="892ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="892ce-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="892ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="892ce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="892ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="892ce-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="892ce-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="892ce-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="892ce-108">Prerequisites</span></span>
<span data-ttu-id="892ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="892ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="892ce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="892ce-111">Permission type</span></span>|<span data-ttu-id="892ce-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="892ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="892ce-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="892ce-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="892ce-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="892ce-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="892ce-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ce-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="892ce-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="892ce-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="892ce-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="892ce-117">Not supported.</span></span>|
|<span data-ttu-id="892ce-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="892ce-118">Application</span></span>||
| <span data-ttu-id="892ce-119">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="892ce-119">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="892ce-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ce-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="892ce-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="892ce-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="892ce-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="892ce-122">Request headers</span></span>
|<span data-ttu-id="892ce-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="892ce-123">Header</span></span>|<span data-ttu-id="892ce-124">Valor</span><span class="sxs-lookup"><span data-stu-id="892ce-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="892ce-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="892ce-125">Authorization</span></span>|<span data-ttu-id="892ce-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="892ce-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="892ce-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="892ce-127">Accept</span></span>|<span data-ttu-id="892ce-128">application/json</span><span class="sxs-lookup"><span data-stu-id="892ce-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="892ce-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="892ce-129">Request body</span></span>
<span data-ttu-id="892ce-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="892ce-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="892ce-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="892ce-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="892ce-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="892ce-132">Property</span></span>|<span data-ttu-id="892ce-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="892ce-133">Type</span></span>|<span data-ttu-id="892ce-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="892ce-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="892ce-135">assignments</span><span class="sxs-lookup"><span data-stu-id="892ce-135">assignments</span></span>|<span data-ttu-id="892ce-136">Conjunto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="892ce-136">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="892ce-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="892ce-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="892ce-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="892ce-138">Response</span></span>
<span data-ttu-id="892ce-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="892ce-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="892ce-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="892ce-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="892ce-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="892ce-141">Request</span></span>
<span data-ttu-id="892ce-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="892ce-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign

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

### <a name="response"></a><span data-ttu-id="892ce-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="892ce-143">Response</span></span>
<span data-ttu-id="892ce-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="892ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








