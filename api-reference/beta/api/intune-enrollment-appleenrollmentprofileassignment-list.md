---
title: Listar appleEnrollmentProfileAssignments
description: Listar Propriedades e relações dos objetos appleEnrollmentProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 636e871495ddc1f5c141541a7de7f86658b011f8
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37525809"
---
# <a name="list-appleenrollmentprofileassignments"></a><span data-ttu-id="1e077-103">Listar appleEnrollmentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="1e077-103">List appleEnrollmentProfileAssignments</span></span>

> <span data-ttu-id="1e077-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e077-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e077-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e077-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e077-106">Listar Propriedades e relações dos objetos [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1e077-106">List properties and relationships of the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e077-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e077-107">Prerequisites</span></span>
<span data-ttu-id="1e077-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e077-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e077-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e077-110">Permission type</span></span>|<span data-ttu-id="1e077-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e077-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e077-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e077-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e077-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e077-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1e077-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e077-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e077-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e077-115">Not supported.</span></span>|
|<span data-ttu-id="1e077-116">Application</span><span class="sxs-lookup"><span data-stu-id="1e077-116">Application</span></span>|<span data-ttu-id="1e077-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e077-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e077-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e077-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1e077-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e077-119">Request headers</span></span>
|<span data-ttu-id="1e077-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e077-120">Header</span></span>|<span data-ttu-id="1e077-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1e077-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e077-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e077-122">Authorization</span></span>|<span data-ttu-id="1e077-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e077-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e077-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e077-124">Accept</span></span>|<span data-ttu-id="1e077-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e077-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e077-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e077-126">Request body</span></span>
<span data-ttu-id="1e077-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e077-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e077-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e077-128">Response</span></span>
<span data-ttu-id="1e077-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e077-129">If successful, this method returns a `200 OK` response code and a collection of [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e077-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e077-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e077-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e077-131">Request</span></span>
<span data-ttu-id="1e077-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e077-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

### <a name="response"></a><span data-ttu-id="1e077-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e077-133">Response</span></span>
<span data-ttu-id="1e077-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e077-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
      "id": "5b603771-3771-5b60-7137-605b7137605b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```






