---
title: Listar termsAndConditionsAssignments
description: Listar propriedades e relações dos objetos termsAndConditionsAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bf9966860a9df75c2ae4aec454cc0979bd331b73
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133553"
---
# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="355ff-103">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="355ff-103">List termsAndConditionsAssignments</span></span>

<span data-ttu-id="355ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="355ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="355ff-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="355ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="355ff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="355ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="355ff-107">Listar propriedades e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="355ff-107">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="355ff-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="355ff-108">Prerequisites</span></span>
<span data-ttu-id="355ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="355ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="355ff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="355ff-111">Permission type</span></span>|<span data-ttu-id="355ff-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="355ff-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="355ff-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="355ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="355ff-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="355ff-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="355ff-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="355ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="355ff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="355ff-116">Not supported.</span></span>|
|<span data-ttu-id="355ff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="355ff-117">Application</span></span>|<span data-ttu-id="355ff-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="355ff-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="355ff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="355ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="355ff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="355ff-120">Request headers</span></span>
|<span data-ttu-id="355ff-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="355ff-121">Header</span></span>|<span data-ttu-id="355ff-122">Valor</span><span class="sxs-lookup"><span data-stu-id="355ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="355ff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="355ff-123">Authorization</span></span>|<span data-ttu-id="355ff-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="355ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="355ff-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="355ff-125">Accept</span></span>|<span data-ttu-id="355ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="355ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="355ff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="355ff-127">Request body</span></span>
<span data-ttu-id="355ff-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="355ff-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="355ff-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="355ff-129">Response</span></span>
<span data-ttu-id="355ff-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="355ff-130">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="355ff-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="355ff-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="355ff-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="355ff-132">Request</span></span>
<span data-ttu-id="355ff-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="355ff-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="355ff-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="355ff-134">Response</span></span>
<span data-ttu-id="355ff-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="355ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 501

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
      "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




