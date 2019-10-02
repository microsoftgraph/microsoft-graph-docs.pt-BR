---
title: Listar enrollmentConfigurationAssignments
description: Listar propriedades e relações de objetos de enrollmentConfigurationAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 325e644ff730c4dad1da6f11c93b2d5124744d6d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362299"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="7d20b-103">Listar enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="7d20b-103">List enrollmentConfigurationAssignments</span></span>

> <span data-ttu-id="7d20b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d20b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d20b-105">Listar propriedades e relações de objetos de [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7d20b-105">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d20b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d20b-106">Prerequisites</span></span>
<span data-ttu-id="7d20b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d20b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d20b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d20b-109">Permission type</span></span>|<span data-ttu-id="7d20b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d20b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d20b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d20b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7d20b-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d20b-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7d20b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d20b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d20b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d20b-114">Not supported.</span></span>|
|<span data-ttu-id="7d20b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d20b-115">Application</span></span>|<span data-ttu-id="7d20b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d20b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d20b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d20b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7d20b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d20b-118">Request headers</span></span>
|<span data-ttu-id="7d20b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d20b-119">Header</span></span>|<span data-ttu-id="7d20b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7d20b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d20b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d20b-121">Authorization</span></span>|<span data-ttu-id="7d20b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d20b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d20b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d20b-123">Accept</span></span>|<span data-ttu-id="7d20b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7d20b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d20b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d20b-125">Request body</span></span>
<span data-ttu-id="7d20b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d20b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d20b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d20b-127">Response</span></span>
<span data-ttu-id="7d20b-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d20b-128">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d20b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d20b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d20b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d20b-130">Request</span></span>
<span data-ttu-id="7d20b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d20b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="7d20b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d20b-132">Response</span></span>
<span data-ttu-id="7d20b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d20b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




