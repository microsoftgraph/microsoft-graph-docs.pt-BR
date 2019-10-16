---
title: ação getPolicySets
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 815c49c6886d22dce0c612f7178acd73ccd9ea07
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536326"
---
# <a name="getpolicysets-action"></a><span data-ttu-id="6a4cd-103">ação getPolicySets</span><span class="sxs-lookup"><span data-stu-id="6a4cd-103">getPolicySets action</span></span>

> <span data-ttu-id="6a4cd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a4cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a4cd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a4cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a4cd-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6a4cd-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a4cd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a4cd-107">Prerequisites</span></span>
<span data-ttu-id="6a4cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a4cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a4cd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a4cd-110">Permission type</span></span>|<span data-ttu-id="6a4cd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a4cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a4cd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a4cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a4cd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a4cd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6a4cd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a4cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a4cd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a4cd-115">Not supported.</span></span>|
|<span data-ttu-id="6a4cd-116">Application</span><span class="sxs-lookup"><span data-stu-id="6a4cd-116">Application</span></span>|<span data-ttu-id="6a4cd-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a4cd-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a4cd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a4cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/getPolicySets
```

## <a name="request-headers"></a><span data-ttu-id="6a4cd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a4cd-119">Request headers</span></span>
|<span data-ttu-id="6a4cd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a4cd-120">Header</span></span>|<span data-ttu-id="6a4cd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6a4cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a4cd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a4cd-122">Authorization</span></span>|<span data-ttu-id="6a4cd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a4cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a4cd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a4cd-124">Accept</span></span>|<span data-ttu-id="6a4cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a4cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a4cd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a4cd-126">Request body</span></span>
<span data-ttu-id="6a4cd-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="6a4cd-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6a4cd-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="6a4cd-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6a4cd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a4cd-129">Property</span></span>|<span data-ttu-id="6a4cd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a4cd-130">Type</span></span>|<span data-ttu-id="6a4cd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a4cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a4cd-132">policySetIds</span><span class="sxs-lookup"><span data-stu-id="6a4cd-132">policySetIds</span></span>|<span data-ttu-id="6a4cd-133">String collection</span><span class="sxs-lookup"><span data-stu-id="6a4cd-133">String collection</span></span>|<span data-ttu-id="6a4cd-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6a4cd-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6a4cd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a4cd-135">Response</span></span>
<span data-ttu-id="6a4cd-136">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [policyset](../resources/intune-policyset-policyset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a4cd-136">If successful, this action returns a `200 OK` response code and a [policySet](../resources/intune-policyset-policyset.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a4cd-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a4cd-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a4cd-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a4cd-138">Request</span></span>
<span data-ttu-id="6a4cd-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a4cd-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6a4cd-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a4cd-140">Response</span></span>
<span data-ttu-id="6a4cd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a4cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






