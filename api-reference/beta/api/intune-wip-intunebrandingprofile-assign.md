---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c463bee7422654430f055822d33b5d59e8540f25
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790316"
---
# <a name="assign-action"></a><span data-ttu-id="be507-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="be507-103">assign action</span></span>

> <span data-ttu-id="be507-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="be507-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be507-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="be507-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be507-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="be507-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be507-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="be507-107">Prerequisites</span></span>
<span data-ttu-id="be507-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be507-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be507-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be507-110">Permission type</span></span>|<span data-ttu-id="be507-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="be507-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be507-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be507-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be507-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be507-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="be507-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be507-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be507-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be507-115">Not supported.</span></span>|
|<span data-ttu-id="be507-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be507-116">Application</span></span>|<span data-ttu-id="be507-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be507-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be507-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be507-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="be507-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be507-119">Request headers</span></span>
|<span data-ttu-id="be507-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be507-120">Header</span></span>|<span data-ttu-id="be507-121">Valor</span><span class="sxs-lookup"><span data-stu-id="be507-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be507-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="be507-122">Authorization</span></span>|<span data-ttu-id="be507-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be507-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be507-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="be507-124">Accept</span></span>|<span data-ttu-id="be507-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be507-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be507-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be507-126">Request body</span></span>
<span data-ttu-id="be507-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="be507-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="be507-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="be507-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="be507-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be507-129">Property</span></span>|<span data-ttu-id="be507-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="be507-130">Type</span></span>|<span data-ttu-id="be507-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="be507-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be507-132">assignments</span><span class="sxs-lookup"><span data-stu-id="be507-132">assignments</span></span>|<span data-ttu-id="be507-133">coleção [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="be507-133">[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) collection</span></span>|<span data-ttu-id="be507-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="be507-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="be507-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="be507-135">Response</span></span>
<span data-ttu-id="be507-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="be507-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="be507-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be507-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="be507-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be507-138">Request</span></span>
<span data-ttu-id="be507-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be507-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assign

Content-type: application/json
Content-length: 279

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
      "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="be507-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="be507-140">Response</span></span>
<span data-ttu-id="be507-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be507-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





