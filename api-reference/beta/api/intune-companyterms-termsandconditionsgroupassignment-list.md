---
title: Listar termsAndConditionsGroupAssignments
description: Listar Propriedades e relações dos objetos termsAndConditionsGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 891b446ead0fd49ec88a199856fa08b507b8a038
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170375"
---
# <a name="list-termsandconditionsgroupassignments"></a><span data-ttu-id="489fb-103">Listar termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="489fb-103">List termsAndConditionsGroupAssignments</span></span>

> <span data-ttu-id="489fb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="489fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="489fb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="489fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="489fb-106">Listar Propriedades e relações dos objetos [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="489fb-106">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="489fb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="489fb-107">Prerequisites</span></span>
<span data-ttu-id="489fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="489fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="489fb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="489fb-110">Permission type</span></span>|<span data-ttu-id="489fb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="489fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="489fb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="489fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="489fb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="489fb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="489fb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="489fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="489fb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="489fb-115">Not supported.</span></span>|
|<span data-ttu-id="489fb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="489fb-116">Application</span></span>|<span data-ttu-id="489fb-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="489fb-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="489fb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="489fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="489fb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="489fb-119">Request headers</span></span>
|<span data-ttu-id="489fb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="489fb-120">Header</span></span>|<span data-ttu-id="489fb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="489fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="489fb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="489fb-122">Authorization</span></span>|<span data-ttu-id="489fb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="489fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="489fb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="489fb-124">Accept</span></span>|<span data-ttu-id="489fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="489fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="489fb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="489fb-126">Request body</span></span>
<span data-ttu-id="489fb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="489fb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="489fb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="489fb-128">Response</span></span>
<span data-ttu-id="489fb-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="489fb-129">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="489fb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="489fb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="489fb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="489fb-131">Request</span></span>
<span data-ttu-id="489fb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="489fb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="489fb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="489fb-133">Response</span></span>
<span data-ttu-id="489fb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="489fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




