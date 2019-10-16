---
title: Listar appleUserInitiatedEnrollmentProfiles
description: Listar Propriedades e relações dos objetos appleUserInitiatedEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ff75b423da77f4e353fe4ca02dc81ee326f2fa34
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37525683"
---
# <a name="list-appleuserinitiatedenrollmentprofiles"></a><span data-ttu-id="ef390-103">Listar appleUserInitiatedEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="ef390-103">List appleUserInitiatedEnrollmentProfiles</span></span>

> <span data-ttu-id="ef390-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ef390-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef390-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef390-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef390-106">Listar Propriedades e relações dos objetos [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ef390-106">List properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef390-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef390-107">Prerequisites</span></span>
<span data-ttu-id="ef390-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef390-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef390-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef390-110">Permission type</span></span>|<span data-ttu-id="ef390-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef390-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef390-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef390-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef390-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef390-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ef390-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef390-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef390-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef390-115">Not supported.</span></span>|
|<span data-ttu-id="ef390-116">Application</span><span class="sxs-lookup"><span data-stu-id="ef390-116">Application</span></span>|<span data-ttu-id="ef390-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef390-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef390-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef390-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/appleUserInitiatedEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="ef390-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef390-119">Request headers</span></span>
|<span data-ttu-id="ef390-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef390-120">Header</span></span>|<span data-ttu-id="ef390-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ef390-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef390-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef390-122">Authorization</span></span>|<span data-ttu-id="ef390-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef390-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef390-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ef390-124">Accept</span></span>|<span data-ttu-id="ef390-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef390-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef390-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef390-126">Request body</span></span>
<span data-ttu-id="ef390-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ef390-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef390-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef390-128">Response</span></span>
<span data-ttu-id="ef390-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef390-129">If successful, this method returns a `200 OK` response code and a collection of [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef390-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef390-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef390-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef390-131">Request</span></span>
<span data-ttu-id="ef390-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef390-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="ef390-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef390-133">Response</span></span>
<span data-ttu-id="ef390-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef390-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 708

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
      "defaultEnrollmentType": "device",
      "availableEnrollmentTypeOptions": [
        {
          "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
          "ownerType": "company",
          "enrollmentType": "device"
        }
      ],
      "id": "5a11d98e-d98e-5a11-8ed9-115a8ed9115a",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "platform": "androidForWork",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```






