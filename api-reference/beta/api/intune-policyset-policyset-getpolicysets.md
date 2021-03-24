---
title: Ação getPolicySets
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fbdf718bd9caac3acb4c8b843d93bffc5a40feb1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134596"
---
# <a name="getpolicysets-action"></a><span data-ttu-id="0e8e2-103">Ação getPolicySets</span><span class="sxs-lookup"><span data-stu-id="0e8e2-103">getPolicySets action</span></span>

<span data-ttu-id="0e8e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e8e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e8e2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e8e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e8e2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e8e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e8e2-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0e8e2-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e8e2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e8e2-108">Prerequisites</span></span>
<span data-ttu-id="0e8e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e8e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e8e2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e8e2-111">Permission type</span></span>|<span data-ttu-id="0e8e2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e8e2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e8e2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e8e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e8e2-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e8e2-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e8e2-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e8e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e8e2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e8e2-116">Not supported.</span></span>|
|<span data-ttu-id="0e8e2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e8e2-117">Application</span></span>|<span data-ttu-id="0e8e2-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e8e2-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e8e2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e8e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/getPolicySets
```

## <a name="request-headers"></a><span data-ttu-id="0e8e2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e8e2-120">Request headers</span></span>
|<span data-ttu-id="0e8e2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e8e2-121">Header</span></span>|<span data-ttu-id="0e8e2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0e8e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e8e2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e8e2-123">Authorization</span></span>|<span data-ttu-id="0e8e2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e8e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e8e2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0e8e2-125">Accept</span></span>|<span data-ttu-id="0e8e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e8e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e8e2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e8e2-127">Request body</span></span>
<span data-ttu-id="0e8e2-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0e8e2-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0e8e2-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="0e8e2-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0e8e2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e8e2-130">Property</span></span>|<span data-ttu-id="0e8e2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e8e2-131">Type</span></span>|<span data-ttu-id="0e8e2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e8e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e8e2-133">policySetIds</span><span class="sxs-lookup"><span data-stu-id="0e8e2-133">policySetIds</span></span>|<span data-ttu-id="0e8e2-134">String collection</span><span class="sxs-lookup"><span data-stu-id="0e8e2-134">String collection</span></span>|<span data-ttu-id="0e8e2-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0e8e2-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0e8e2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e8e2-136">Response</span></span>
<span data-ttu-id="0e8e2-137">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e uma coleção [policySet](../resources/intune-policyset-policyset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e8e2-137">If successful, this action returns a `200 OK` response code and a [policySet](../resources/intune-policyset-policyset.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e8e2-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e8e2-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e8e2-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e8e2-139">Request</span></span>
<span data-ttu-id="0e8e2-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e8e2-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0e8e2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e8e2-141">Response</span></span>
<span data-ttu-id="0e8e2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e8e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




