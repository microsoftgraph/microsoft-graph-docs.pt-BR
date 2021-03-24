---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6efe6ba1b7be0ae05609e9e38da18e31d9cd2e33
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135590"
---
# <a name="assign-action"></a><span data-ttu-id="dd962-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="dd962-103">assign action</span></span>

<span data-ttu-id="dd962-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd962-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd962-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dd962-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd962-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dd962-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd962-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dd962-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd962-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dd962-108">Prerequisites</span></span>
<span data-ttu-id="dd962-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd962-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd962-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd962-111">Permission type</span></span>|<span data-ttu-id="dd962-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd962-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd962-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd962-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd962-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd962-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd962-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd962-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd962-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd962-116">Not supported.</span></span>|
|<span data-ttu-id="dd962-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd962-117">Application</span></span>|<span data-ttu-id="dd962-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd962-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd962-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd962-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="dd962-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd962-120">Request headers</span></span>
|<span data-ttu-id="dd962-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dd962-121">Header</span></span>|<span data-ttu-id="dd962-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dd962-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd962-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd962-123">Authorization</span></span>|<span data-ttu-id="dd962-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd962-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd962-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dd962-125">Accept</span></span>|<span data-ttu-id="dd962-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd962-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd962-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd962-127">Request body</span></span>
<span data-ttu-id="dd962-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="dd962-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dd962-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="dd962-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dd962-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd962-130">Property</span></span>|<span data-ttu-id="dd962-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd962-131">Type</span></span>|<span data-ttu-id="dd962-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd962-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd962-133">assignments</span><span class="sxs-lookup"><span data-stu-id="dd962-133">assignments</span></span>|<span data-ttu-id="dd962-134">[Coleção embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)</span><span class="sxs-lookup"><span data-stu-id="dd962-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="dd962-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dd962-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dd962-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd962-136">Response</span></span>
<span data-ttu-id="dd962-137">Se tiver êxito, essa ação retornará um código de resposta e uma `200 OK` [coleção embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd962-137">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd962-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd962-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd962-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd962-139">Request</span></span>
<span data-ttu-id="dd962-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd962-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign

Content-type: application/json
Content-length: 456

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="dd962-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd962-141">Response</span></span>
<span data-ttu-id="dd962-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd962-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```




