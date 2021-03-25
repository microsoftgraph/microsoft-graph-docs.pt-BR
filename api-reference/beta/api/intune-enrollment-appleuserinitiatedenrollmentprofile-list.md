---
title: Listar appleUserInitiatedEnrollmentProfiles
description: Listar propriedades e relações dos objetos appleUserInitiatedEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 771f08deb1b6000e1fb94bf4a8c3447f68d7ee56
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157665"
---
# <a name="list-appleuserinitiatedenrollmentprofiles"></a><span data-ttu-id="78579-103">Listar appleUserInitiatedEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="78579-103">List appleUserInitiatedEnrollmentProfiles</span></span>

<span data-ttu-id="78579-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78579-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78579-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78579-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78579-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78579-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78579-107">Listar propriedades e relações dos [objetos appleUserInitiatedEnrollmentProfile.](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78579-107">List properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78579-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78579-108">Prerequisites</span></span>
<span data-ttu-id="78579-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78579-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78579-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78579-111">Permission type</span></span>|<span data-ttu-id="78579-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78579-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78579-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78579-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78579-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78579-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="78579-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78579-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78579-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78579-116">Not supported.</span></span>|
|<span data-ttu-id="78579-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78579-117">Application</span></span>|<span data-ttu-id="78579-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78579-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78579-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78579-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/appleUserInitiatedEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="78579-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78579-120">Request headers</span></span>
|<span data-ttu-id="78579-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78579-121">Header</span></span>|<span data-ttu-id="78579-122">Valor</span><span class="sxs-lookup"><span data-stu-id="78579-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78579-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="78579-123">Authorization</span></span>|<span data-ttu-id="78579-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78579-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78579-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78579-125">Accept</span></span>|<span data-ttu-id="78579-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78579-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78579-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78579-127">Request body</span></span>
<span data-ttu-id="78579-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78579-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78579-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="78579-129">Response</span></span>
<span data-ttu-id="78579-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78579-130">If successful, this method returns a `200 OK` response code and a collection of [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78579-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78579-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="78579-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78579-132">Request</span></span>
<span data-ttu-id="78579-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78579-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="78579-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="78579-134">Response</span></span>
<span data-ttu-id="78579-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78579-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




