---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cddbaa0bd40f83b7a9a5160f55dc4a4d2fa750c5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990075"
---
# <a name="assign-action"></a><span data-ttu-id="4afda-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="4afda-103">assign action</span></span>

> <span data-ttu-id="4afda-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4afda-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4afda-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4afda-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4afda-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4afda-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4afda-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4afda-107">Prerequisites</span></span>
<span data-ttu-id="4afda-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4afda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4afda-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4afda-110">Permission type</span></span>|<span data-ttu-id="4afda-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4afda-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4afda-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4afda-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4afda-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4afda-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4afda-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4afda-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4afda-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4afda-115">Not supported.</span></span>|
|<span data-ttu-id="4afda-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4afda-116">Application</span></span>|<span data-ttu-id="4afda-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4afda-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4afda-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4afda-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="4afda-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4afda-119">Request headers</span></span>
|<span data-ttu-id="4afda-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4afda-120">Header</span></span>|<span data-ttu-id="4afda-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4afda-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4afda-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4afda-122">Authorization</span></span>|<span data-ttu-id="4afda-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4afda-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4afda-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4afda-124">Accept</span></span>|<span data-ttu-id="4afda-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4afda-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4afda-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4afda-126">Request body</span></span>
<span data-ttu-id="4afda-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="4afda-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4afda-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="4afda-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4afda-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4afda-129">Property</span></span>|<span data-ttu-id="4afda-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4afda-130">Type</span></span>|<span data-ttu-id="4afda-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4afda-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4afda-132">assignments</span><span class="sxs-lookup"><span data-stu-id="4afda-132">assignments</span></span>|<span data-ttu-id="4afda-133">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4afda-133">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4afda-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4afda-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4afda-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4afda-135">Response</span></span>
<span data-ttu-id="4afda-136">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4afda-136">If successful, this action returns a `200 OK` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4afda-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4afda-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="4afda-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4afda-138">Request</span></span>
<span data-ttu-id="4afda-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4afda-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign

Content-type: application/json
Content-length: 350

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4afda-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4afda-140">Response</span></span>
<span data-ttu-id="4afda-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4afda-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





