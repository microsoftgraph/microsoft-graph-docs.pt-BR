---
title: Ação updateDeviceProfileAssignment
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b4634087eb69e9d3f0f7b1060837b977f02f0313
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142419"
---
# <a name="updatedeviceprofileassignment-action"></a><span data-ttu-id="21cfb-103">Ação updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="21cfb-103">updateDeviceProfileAssignment action</span></span>

<span data-ttu-id="21cfb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21cfb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21cfb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21cfb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21cfb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21cfb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21cfb-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="21cfb-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21cfb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21cfb-108">Prerequisites</span></span>
<span data-ttu-id="21cfb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21cfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21cfb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21cfb-111">Permission type</span></span>|<span data-ttu-id="21cfb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21cfb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21cfb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21cfb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21cfb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21cfb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="21cfb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21cfb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21cfb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21cfb-116">Not supported.</span></span>|
|<span data-ttu-id="21cfb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21cfb-117">Application</span></span>|<span data-ttu-id="21cfb-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21cfb-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21cfb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21cfb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/updateDeviceProfileAssignment
```

## <a name="request-headers"></a><span data-ttu-id="21cfb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21cfb-120">Request headers</span></span>
|<span data-ttu-id="21cfb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21cfb-121">Header</span></span>|<span data-ttu-id="21cfb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="21cfb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21cfb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="21cfb-123">Authorization</span></span>|<span data-ttu-id="21cfb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21cfb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21cfb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21cfb-125">Accept</span></span>|<span data-ttu-id="21cfb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21cfb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21cfb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21cfb-127">Request body</span></span>
<span data-ttu-id="21cfb-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="21cfb-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="21cfb-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="21cfb-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="21cfb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21cfb-130">Property</span></span>|<span data-ttu-id="21cfb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="21cfb-131">Type</span></span>|<span data-ttu-id="21cfb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="21cfb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21cfb-133">deviceIds</span><span class="sxs-lookup"><span data-stu-id="21cfb-133">deviceIds</span></span>|<span data-ttu-id="21cfb-134">String collection</span><span class="sxs-lookup"><span data-stu-id="21cfb-134">String collection</span></span>|<span data-ttu-id="21cfb-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="21cfb-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="21cfb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="21cfb-136">Response</span></span>
<span data-ttu-id="21cfb-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="21cfb-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="21cfb-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21cfb-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="21cfb-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21cfb-139">Request</span></span>
<span data-ttu-id="21cfb-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21cfb-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/updateDeviceProfileAssignment

Content-type: application/json
Content-length: 51

{
  "deviceIds": [
    "Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="21cfb-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="21cfb-141">Response</span></span>
<span data-ttu-id="21cfb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21cfb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




