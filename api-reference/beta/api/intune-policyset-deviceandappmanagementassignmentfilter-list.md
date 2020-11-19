---
title: Listar deviceAndAppManagementAssignmentFilters
description: Listar Propriedades e relações dos objetos deviceAndAppManagementAssignmentFilter.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e87df7e4945b181525e5e280873fc83c596d15fe
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49224197"
---
# <a name="list-deviceandappmanagementassignmentfilters"></a><span data-ttu-id="25267-103">Listar deviceAndAppManagementAssignmentFilters</span><span class="sxs-lookup"><span data-stu-id="25267-103">List deviceAndAppManagementAssignmentFilters</span></span>

<span data-ttu-id="25267-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25267-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25267-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="25267-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25267-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25267-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25267-107">Listar Propriedades e relações dos objetos [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) .</span><span class="sxs-lookup"><span data-stu-id="25267-107">List properties and relationships of the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25267-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="25267-108">Prerequisites</span></span>
<span data-ttu-id="25267-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25267-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25267-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25267-111">Permission type</span></span>|<span data-ttu-id="25267-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="25267-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25267-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25267-113">Delegated (work or school account)</span></span>|<span data-ttu-id="25267-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="25267-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="25267-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25267-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25267-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25267-116">Not supported.</span></span>|
|<span data-ttu-id="25267-117">Application</span><span class="sxs-lookup"><span data-stu-id="25267-117">Application</span></span>|<span data-ttu-id="25267-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="25267-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25267-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25267-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/assignmentFilters
```

## <a name="request-headers"></a><span data-ttu-id="25267-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25267-120">Request headers</span></span>
|<span data-ttu-id="25267-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25267-121">Header</span></span>|<span data-ttu-id="25267-122">Valor</span><span class="sxs-lookup"><span data-stu-id="25267-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25267-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="25267-123">Authorization</span></span>|<span data-ttu-id="25267-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25267-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25267-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="25267-125">Accept</span></span>|<span data-ttu-id="25267-126">application/json</span><span class="sxs-lookup"><span data-stu-id="25267-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25267-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25267-127">Request body</span></span>
<span data-ttu-id="25267-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25267-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25267-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="25267-129">Response</span></span>
<span data-ttu-id="25267-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25267-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25267-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25267-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="25267-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25267-132">Request</span></span>
<span data-ttu-id="25267-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25267-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/assignmentFilters
```

### <a name="response"></a><span data-ttu-id="25267-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="25267-134">Response</span></span>
<span data-ttu-id="25267-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25267-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 523

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
      "id": "819818db-18db-8198-db18-9881db189881",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "platform": "androidForWork",
      "rule": "Rule value",
      "roleScopeTags": [
        "Role Scope Tags value"
      ]
    }
  ]
}
```




