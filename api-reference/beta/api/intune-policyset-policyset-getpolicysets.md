---
title: ação getPolicySets
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e91eb9162ba373f8737371c306df7522112f2c3b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191739"
---
# <a name="getpolicysets-action"></a><span data-ttu-id="0c97b-103">ação getPolicySets</span><span class="sxs-lookup"><span data-stu-id="0c97b-103">getPolicySets action</span></span>

> <span data-ttu-id="0c97b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0c97b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c97b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c97b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c97b-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0c97b-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c97b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c97b-107">Prerequisites</span></span>
<span data-ttu-id="0c97b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c97b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c97b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c97b-110">Permission type</span></span>|<span data-ttu-id="0c97b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c97b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c97b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c97b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c97b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c97b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0c97b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c97b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c97b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c97b-115">Not supported.</span></span>|
|<span data-ttu-id="0c97b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c97b-116">Application</span></span>|<span data-ttu-id="0c97b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c97b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c97b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c97b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/getPolicySets
```

## <a name="request-headers"></a><span data-ttu-id="0c97b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c97b-119">Request headers</span></span>
|<span data-ttu-id="0c97b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c97b-120">Header</span></span>|<span data-ttu-id="0c97b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0c97b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c97b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c97b-122">Authorization</span></span>|<span data-ttu-id="0c97b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c97b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c97b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c97b-124">Accept</span></span>|<span data-ttu-id="0c97b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c97b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c97b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c97b-126">Request body</span></span>
<span data-ttu-id="0c97b-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0c97b-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0c97b-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="0c97b-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0c97b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c97b-129">Property</span></span>|<span data-ttu-id="0c97b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c97b-130">Type</span></span>|<span data-ttu-id="0c97b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c97b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c97b-132">policySetIds</span><span class="sxs-lookup"><span data-stu-id="0c97b-132">policySetIds</span></span>|<span data-ttu-id="0c97b-133">String collection</span><span class="sxs-lookup"><span data-stu-id="0c97b-133">String collection</span></span>|<span data-ttu-id="0c97b-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0c97b-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0c97b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c97b-135">Response</span></span>
<span data-ttu-id="0c97b-136">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [policyset](../resources/intune-policyset-policyset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c97b-136">If successful, this action returns a `200 OK` response code and a [policySet](../resources/intune-policyset-policyset.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c97b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c97b-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c97b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c97b-138">Request</span></span>
<span data-ttu-id="0c97b-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c97b-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/getPolicySets

Content-type: application/json
Content-length: 58

{
  "policySetIds": [
    "Policy Set Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="0c97b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c97b-140">Response</span></span>
<span data-ttu-id="0c97b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c97b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 578

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.policySet",
      "id": "653cb373-b373-653c-73b3-3c6573b33c65",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ],
      "roleScopeTags": [
        "Role Scope Tags value"
      ]
    }
  ]
}
```




