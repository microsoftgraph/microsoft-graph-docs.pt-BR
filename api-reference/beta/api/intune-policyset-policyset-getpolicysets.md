---
title: ação getPolicySets
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c8ed1488551d4f4ebf0e4ac7d04d36dbf48e40d6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460553"
---
# <a name="getpolicysets-action"></a><span data-ttu-id="a8938-103">ação getPolicySets</span><span class="sxs-lookup"><span data-stu-id="a8938-103">getPolicySets action</span></span>

<span data-ttu-id="a8938-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a8938-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8938-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8938-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8938-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8938-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8938-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a8938-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8938-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8938-108">Prerequisites</span></span>
<span data-ttu-id="a8938-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8938-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8938-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8938-111">Permission type</span></span>|<span data-ttu-id="a8938-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a8938-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8938-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8938-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8938-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8938-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a8938-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8938-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8938-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8938-116">Not supported.</span></span>|
|<span data-ttu-id="a8938-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8938-117">Application</span></span>|<span data-ttu-id="a8938-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8938-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8938-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8938-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/getPolicySets
```

## <a name="request-headers"></a><span data-ttu-id="a8938-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8938-120">Request headers</span></span>
|<span data-ttu-id="a8938-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8938-121">Header</span></span>|<span data-ttu-id="a8938-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a8938-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8938-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8938-123">Authorization</span></span>|<span data-ttu-id="a8938-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8938-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8938-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a8938-125">Accept</span></span>|<span data-ttu-id="a8938-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8938-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8938-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8938-127">Request body</span></span>
<span data-ttu-id="a8938-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a8938-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a8938-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="a8938-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a8938-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8938-130">Property</span></span>|<span data-ttu-id="a8938-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8938-131">Type</span></span>|<span data-ttu-id="a8938-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8938-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8938-133">policySetIds</span><span class="sxs-lookup"><span data-stu-id="a8938-133">policySetIds</span></span>|<span data-ttu-id="a8938-134">String collection</span><span class="sxs-lookup"><span data-stu-id="a8938-134">String collection</span></span>|<span data-ttu-id="a8938-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a8938-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a8938-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8938-136">Response</span></span>
<span data-ttu-id="a8938-137">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [policyset](../resources/intune-policyset-policyset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8938-137">If successful, this action returns a `200 OK` response code and a [policySet](../resources/intune-policyset-policyset.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8938-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8938-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8938-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8938-139">Request</span></span>
<span data-ttu-id="a8938-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8938-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a8938-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8938-141">Response</span></span>
<span data-ttu-id="a8938-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8938-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





