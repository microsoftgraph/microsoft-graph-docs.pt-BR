---
title: Listar appleUserInitiatedEnrollmentProfiles
description: Listar Propriedades e relações dos objetos appleUserInitiatedEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f14af292fc712c13b1e8e066e0c0bb9829185652
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49309709"
---
# <a name="list-appleuserinitiatedenrollmentprofiles"></a><span data-ttu-id="aba35-103">Listar appleUserInitiatedEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="aba35-103">List appleUserInitiatedEnrollmentProfiles</span></span>

<span data-ttu-id="aba35-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aba35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aba35-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aba35-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aba35-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aba35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aba35-107">Listar Propriedades e relações dos objetos [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="aba35-107">List properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aba35-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aba35-108">Prerequisites</span></span>
<span data-ttu-id="aba35-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aba35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aba35-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aba35-111">Permission type</span></span>|<span data-ttu-id="aba35-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aba35-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aba35-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aba35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aba35-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="aba35-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="aba35-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aba35-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aba35-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aba35-116">Not supported.</span></span>|
|<span data-ttu-id="aba35-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aba35-117">Application</span></span>|<span data-ttu-id="aba35-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="aba35-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aba35-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aba35-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/appleUserInitiatedEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="aba35-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aba35-120">Request headers</span></span>
|<span data-ttu-id="aba35-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aba35-121">Header</span></span>|<span data-ttu-id="aba35-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aba35-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aba35-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aba35-123">Authorization</span></span>|<span data-ttu-id="aba35-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aba35-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aba35-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aba35-125">Accept</span></span>|<span data-ttu-id="aba35-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aba35-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aba35-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aba35-127">Request body</span></span>
<span data-ttu-id="aba35-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aba35-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aba35-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="aba35-129">Response</span></span>
<span data-ttu-id="aba35-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aba35-130">If successful, this method returns a `200 OK` response code and a collection of [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aba35-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aba35-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="aba35-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aba35-132">Request</span></span>
<span data-ttu-id="aba35-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aba35-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="aba35-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="aba35-134">Response</span></span>
<span data-ttu-id="aba35-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aba35-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




