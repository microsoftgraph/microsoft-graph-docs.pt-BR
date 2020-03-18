---
title: Listar enrollmentConfigurationAssignments
description: Listar propriedades e relações de objetos de enrollmentConfigurationAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 109300f63c95f55a59524371f3a659692b8ae418
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802822"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="83a58-103">Listar enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="83a58-103">List enrollmentConfigurationAssignments</span></span>

> <span data-ttu-id="83a58-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83a58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83a58-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83a58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83a58-106">Listar propriedades e relações de objetos de [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="83a58-106">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83a58-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="83a58-107">Prerequisites</span></span>
<span data-ttu-id="83a58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83a58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83a58-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83a58-110">Permission type</span></span>|<span data-ttu-id="83a58-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="83a58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83a58-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83a58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="83a58-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="83a58-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="83a58-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83a58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83a58-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83a58-115">Not supported.</span></span>|
|<span data-ttu-id="83a58-116">Application</span><span class="sxs-lookup"><span data-stu-id="83a58-116">Application</span></span>|<span data-ttu-id="83a58-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="83a58-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83a58-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83a58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="83a58-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83a58-119">Request headers</span></span>
|<span data-ttu-id="83a58-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83a58-120">Header</span></span>|<span data-ttu-id="83a58-121">Valor</span><span class="sxs-lookup"><span data-stu-id="83a58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83a58-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="83a58-122">Authorization</span></span>|<span data-ttu-id="83a58-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83a58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83a58-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="83a58-124">Accept</span></span>|<span data-ttu-id="83a58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="83a58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83a58-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83a58-126">Request body</span></span>
<span data-ttu-id="83a58-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83a58-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83a58-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="83a58-128">Response</span></span>
<span data-ttu-id="83a58-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83a58-129">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83a58-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83a58-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="83a58-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83a58-131">Request</span></span>
<span data-ttu-id="83a58-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83a58-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="83a58-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="83a58-133">Response</span></span>
<span data-ttu-id="83a58-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83a58-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```




