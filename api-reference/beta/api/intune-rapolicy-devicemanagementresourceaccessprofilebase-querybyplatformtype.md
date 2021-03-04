---
title: ação queryByPlatformType
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cfef02eac2586fc98f8a86f9e7740b654695e14f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445921"
---
# <a name="querybyplatformtype-action"></a><span data-ttu-id="9bfbd-103">ação queryByPlatformType</span><span class="sxs-lookup"><span data-stu-id="9bfbd-103">queryByPlatformType action</span></span>

<span data-ttu-id="9bfbd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bfbd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bfbd-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9bfbd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bfbd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9bfbd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bfbd-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9bfbd-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bfbd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9bfbd-108">Prerequisites</span></span>
<span data-ttu-id="9bfbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bfbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bfbd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bfbd-111">Permission type</span></span>|<span data-ttu-id="9bfbd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9bfbd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bfbd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bfbd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9bfbd-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bfbd-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9bfbd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bfbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bfbd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bfbd-116">Not supported.</span></span>|
|<span data-ttu-id="9bfbd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bfbd-117">Application</span></span>|<span data-ttu-id="9bfbd-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bfbd-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bfbd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bfbd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles/queryByPlatformType
```

## <a name="request-headers"></a><span data-ttu-id="9bfbd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bfbd-120">Request headers</span></span>
|<span data-ttu-id="9bfbd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9bfbd-121">Header</span></span>|<span data-ttu-id="9bfbd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9bfbd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bfbd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bfbd-123">Authorization</span></span>|<span data-ttu-id="9bfbd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bfbd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bfbd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9bfbd-125">Accept</span></span>|<span data-ttu-id="9bfbd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9bfbd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bfbd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bfbd-127">Request body</span></span>
<span data-ttu-id="9bfbd-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9bfbd-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9bfbd-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="9bfbd-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9bfbd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bfbd-130">Property</span></span>|<span data-ttu-id="9bfbd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bfbd-131">Type</span></span>|<span data-ttu-id="9bfbd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bfbd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bfbd-133">platformType</span><span class="sxs-lookup"><span data-stu-id="9bfbd-133">platformType</span></span>|[<span data-ttu-id="9bfbd-134">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="9bfbd-134">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="9bfbd-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9bfbd-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9bfbd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bfbd-136">Response</span></span>
<span data-ttu-id="9bfbd-137">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um [iQueryable_1OfDeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-iqueryable_1ofdevicemanagementresourceaccessprofilebase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bfbd-137">If successful, this action returns a `200 OK` response code and a [iQueryable_1OfDeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-iqueryable_1ofdevicemanagementresourceaccessprofilebase.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bfbd-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bfbd-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bfbd-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bfbd-139">Request</span></span>
<span data-ttu-id="9bfbd-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bfbd-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/queryByPlatformType

Content-type: application/json
Content-length: 40

{
  "platformType": "androidForWork"
}
```

### <a name="response"></a><span data-ttu-id="9bfbd-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bfbd-141">Response</span></span>
<span data-ttu-id="9bfbd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bfbd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 117

{
  "value": {
    "@odata.type": "microsoft.graph.iQueryable_1OfDeviceManagementResourceAccessProfileBase"
  }
}
```




