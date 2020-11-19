---
title: ação getPolicySets
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a7790ac7bc283cb60e7287aa48202b489bd8bb33
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49296164"
---
# <a name="getpolicysets-action"></a><span data-ttu-id="d93e9-103">ação getPolicySets</span><span class="sxs-lookup"><span data-stu-id="d93e9-103">getPolicySets action</span></span>

<span data-ttu-id="d93e9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d93e9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d93e9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d93e9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d93e9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d93e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d93e9-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d93e9-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d93e9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d93e9-108">Prerequisites</span></span>
<span data-ttu-id="d93e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d93e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d93e9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d93e9-111">Permission type</span></span>|<span data-ttu-id="d93e9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d93e9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d93e9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d93e9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d93e9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d93e9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d93e9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d93e9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d93e9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d93e9-116">Not supported.</span></span>|
|<span data-ttu-id="d93e9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d93e9-117">Application</span></span>|<span data-ttu-id="d93e9-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d93e9-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d93e9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d93e9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/getPolicySets
```

## <a name="request-headers"></a><span data-ttu-id="d93e9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d93e9-120">Request headers</span></span>
|<span data-ttu-id="d93e9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d93e9-121">Header</span></span>|<span data-ttu-id="d93e9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d93e9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d93e9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d93e9-123">Authorization</span></span>|<span data-ttu-id="d93e9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d93e9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d93e9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d93e9-125">Accept</span></span>|<span data-ttu-id="d93e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d93e9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d93e9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d93e9-127">Request body</span></span>
<span data-ttu-id="d93e9-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d93e9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d93e9-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d93e9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d93e9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d93e9-130">Property</span></span>|<span data-ttu-id="d93e9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d93e9-131">Type</span></span>|<span data-ttu-id="d93e9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d93e9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d93e9-133">policySetIds</span><span class="sxs-lookup"><span data-stu-id="d93e9-133">policySetIds</span></span>|<span data-ttu-id="d93e9-134">String collection</span><span class="sxs-lookup"><span data-stu-id="d93e9-134">String collection</span></span>|<span data-ttu-id="d93e9-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d93e9-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d93e9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d93e9-136">Response</span></span>
<span data-ttu-id="d93e9-137">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e uma coleção [policyset](../resources/intune-policyset-policyset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d93e9-137">If successful, this action returns a `200 OK` response code and a [policySet](../resources/intune-policyset-policyset.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d93e9-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d93e9-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d93e9-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d93e9-139">Request</span></span>
<span data-ttu-id="d93e9-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d93e9-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d93e9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d93e9-141">Response</span></span>
<span data-ttu-id="d93e9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d93e9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




