---
title: Listar termsAndConditionsGroupAssignments
description: Listar Propriedades e relações dos objetos termsAndConditionsGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0fdfc47a1f12b57db29679ad1ab9ac11519aa716
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144601"
---
# <a name="list-termsandconditionsgroupassignments"></a><span data-ttu-id="2816f-103">Listar termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="2816f-103">List termsAndConditionsGroupAssignments</span></span>

> <span data-ttu-id="2816f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2816f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2816f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2816f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2816f-106">Listar Propriedades e relações dos objetos [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2816f-106">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2816f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2816f-107">Prerequisites</span></span>
<span data-ttu-id="2816f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2816f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2816f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2816f-110">Permission type</span></span>|<span data-ttu-id="2816f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2816f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2816f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2816f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2816f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2816f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2816f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2816f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2816f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2816f-115">Not supported.</span></span>|
|<span data-ttu-id="2816f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2816f-116">Application</span></span>|<span data-ttu-id="2816f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2816f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2816f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2816f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="2816f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2816f-119">Request headers</span></span>
|<span data-ttu-id="2816f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2816f-120">Header</span></span>|<span data-ttu-id="2816f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2816f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2816f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2816f-122">Authorization</span></span>|<span data-ttu-id="2816f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2816f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2816f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2816f-124">Accept</span></span>|<span data-ttu-id="2816f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2816f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2816f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2816f-126">Request body</span></span>
<span data-ttu-id="2816f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2816f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2816f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2816f-128">Response</span></span>
<span data-ttu-id="2816f-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2816f-129">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2816f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2816f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2816f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2816f-131">Request</span></span>
<span data-ttu-id="2816f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2816f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="2816f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2816f-133">Response</span></span>
<span data-ttu-id="2816f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2816f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 214

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
      "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
      "targetGroupId": "Target Group Id value"
    }
  ]
}
```




