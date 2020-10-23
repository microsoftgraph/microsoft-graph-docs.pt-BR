---
title: Excluir intuneBrandingProfileAssignment
description: Exclui intuneBrandingProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fff51f6feeb8657dcdb859b65b0f5d7699e5215c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709016"
---
# <a name="delete-intunebrandingprofileassignment"></a><span data-ttu-id="5434f-103">Excluir intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="5434f-103">Delete intuneBrandingProfileAssignment</span></span>

<span data-ttu-id="5434f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5434f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5434f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5434f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5434f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5434f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5434f-107">Exclui [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5434f-107">Deletes a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5434f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5434f-108">Prerequisites</span></span>
<span data-ttu-id="5434f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5434f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5434f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5434f-111">Permission type</span></span>|<span data-ttu-id="5434f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5434f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5434f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5434f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5434f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5434f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5434f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5434f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5434f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5434f-116">Not supported.</span></span>|
|<span data-ttu-id="5434f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5434f-117">Application</span></span>|<span data-ttu-id="5434f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5434f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5434f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5434f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5434f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5434f-120">Request headers</span></span>
|<span data-ttu-id="5434f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5434f-121">Header</span></span>|<span data-ttu-id="5434f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5434f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5434f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5434f-123">Authorization</span></span>|<span data-ttu-id="5434f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5434f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5434f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5434f-125">Accept</span></span>|<span data-ttu-id="5434f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5434f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5434f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5434f-127">Request body</span></span>
<span data-ttu-id="5434f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5434f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5434f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5434f-129">Response</span></span>
<span data-ttu-id="5434f-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5434f-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5434f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5434f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5434f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5434f-132">Request</span></span>
<span data-ttu-id="5434f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5434f-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="5434f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5434f-134">Response</span></span>
<span data-ttu-id="5434f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5434f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





