---
title: ação getPolicySets
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d2908866f28eceb9e50467566c41fc0b7f65b59e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802122"
---
# <a name="getpolicysets-action"></a><span data-ttu-id="75e03-103">ação getPolicySets</span><span class="sxs-lookup"><span data-stu-id="75e03-103">getPolicySets action</span></span>

> <span data-ttu-id="75e03-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75e03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75e03-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75e03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75e03-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="75e03-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75e03-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75e03-107">Prerequisites</span></span>
<span data-ttu-id="75e03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75e03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75e03-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75e03-110">Permission type</span></span>|<span data-ttu-id="75e03-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="75e03-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75e03-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75e03-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75e03-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="75e03-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="75e03-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75e03-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75e03-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75e03-115">Not supported.</span></span>|
|<span data-ttu-id="75e03-116">Application</span><span class="sxs-lookup"><span data-stu-id="75e03-116">Application</span></span>|<span data-ttu-id="75e03-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="75e03-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75e03-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75e03-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/getPolicySets
```

## <a name="request-headers"></a><span data-ttu-id="75e03-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75e03-119">Request headers</span></span>
|<span data-ttu-id="75e03-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75e03-120">Header</span></span>|<span data-ttu-id="75e03-121">Valor</span><span class="sxs-lookup"><span data-stu-id="75e03-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75e03-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="75e03-122">Authorization</span></span>|<span data-ttu-id="75e03-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75e03-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75e03-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75e03-124">Accept</span></span>|<span data-ttu-id="75e03-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75e03-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75e03-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75e03-126">Request body</span></span>
<span data-ttu-id="75e03-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="75e03-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="75e03-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="75e03-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="75e03-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75e03-129">Property</span></span>|<span data-ttu-id="75e03-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="75e03-130">Type</span></span>|<span data-ttu-id="75e03-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="75e03-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75e03-132">policySetIds</span><span class="sxs-lookup"><span data-stu-id="75e03-132">policySetIds</span></span>|<span data-ttu-id="75e03-133">String collection</span><span class="sxs-lookup"><span data-stu-id="75e03-133">String collection</span></span>|<span data-ttu-id="75e03-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="75e03-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="75e03-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="75e03-135">Response</span></span>
<span data-ttu-id="75e03-136">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [policyset](../resources/intune-policyset-policyset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75e03-136">If successful, this action returns a `200 OK` response code and a [policySet](../resources/intune-policyset-policyset.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75e03-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75e03-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="75e03-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75e03-138">Request</span></span>
<span data-ttu-id="75e03-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75e03-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="75e03-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="75e03-140">Response</span></span>
<span data-ttu-id="75e03-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75e03-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




