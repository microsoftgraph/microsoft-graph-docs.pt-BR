---
title: Listar windowsQualityUpdateProfileAssignments
description: Listar propriedades e relações dos objetos windowsQualityUpdateProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d690cb3bdc40430f72820a49afde0ea595d7fc9b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160106"
---
# <a name="list-windowsqualityupdateprofileassignments"></a><span data-ttu-id="7da25-103">Listar windowsQualityUpdateProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="7da25-103">List windowsQualityUpdateProfileAssignments</span></span>

<span data-ttu-id="7da25-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7da25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7da25-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7da25-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7da25-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7da25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7da25-107">Listar propriedades e relações dos [objetos windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7da25-107">List properties and relationships of the [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7da25-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7da25-108">Prerequisites</span></span>
<span data-ttu-id="7da25-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7da25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7da25-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7da25-111">Permission type</span></span>|<span data-ttu-id="7da25-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7da25-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7da25-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7da25-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7da25-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7da25-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7da25-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7da25-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7da25-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7da25-116">Not supported.</span></span>|
|<span data-ttu-id="7da25-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7da25-117">Application</span></span>|<span data-ttu-id="7da25-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7da25-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7da25-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7da25-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7da25-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7da25-120">Request headers</span></span>
|<span data-ttu-id="7da25-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7da25-121">Header</span></span>|<span data-ttu-id="7da25-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7da25-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7da25-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7da25-123">Authorization</span></span>|<span data-ttu-id="7da25-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7da25-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7da25-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7da25-125">Accept</span></span>|<span data-ttu-id="7da25-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7da25-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7da25-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7da25-127">Request body</span></span>
<span data-ttu-id="7da25-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7da25-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7da25-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7da25-129">Response</span></span>
<span data-ttu-id="7da25-130">Se bem-sucedido, este método retorna um código de resposta e uma coleção de `200 OK` [objetos windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7da25-130">If successful, this method returns a `200 OK` response code and a collection of [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7da25-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7da25-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7da25-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7da25-132">Request</span></span>
<span data-ttu-id="7da25-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7da25-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}/assignments
```

### <a name="response"></a><span data-ttu-id="7da25-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7da25-134">Response</span></span>
<span data-ttu-id="7da25-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7da25-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 454

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
      "id": "0c3a8422-8422-0c3a-2284-3a0c22843a0c",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```




