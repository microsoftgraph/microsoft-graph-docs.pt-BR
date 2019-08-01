---
title: Listar termsAndConditionsAssignments
description: Listar propriedades e relações dos objetos termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 85cdd361fd8dbf454e6d01c91ca00e7d39e032d1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020399"
---
# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="41f11-103">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="41f11-103">List termsAndConditionsAssignments</span></span>

> <span data-ttu-id="41f11-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41f11-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41f11-105">Listar propriedades e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="41f11-105">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41f11-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41f11-106">Prerequisites</span></span>
<span data-ttu-id="41f11-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41f11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41f11-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41f11-109">Permission type</span></span>|<span data-ttu-id="41f11-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41f11-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41f11-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41f11-111">Delegated (work or school account)</span></span>|<span data-ttu-id="41f11-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="41f11-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="41f11-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41f11-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41f11-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41f11-114">Not supported.</span></span>|
|<span data-ttu-id="41f11-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41f11-115">Application</span></span>|<span data-ttu-id="41f11-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41f11-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41f11-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41f11-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="41f11-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41f11-118">Request headers</span></span>
|<span data-ttu-id="41f11-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41f11-119">Header</span></span>|<span data-ttu-id="41f11-120">Valor</span><span class="sxs-lookup"><span data-stu-id="41f11-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41f11-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="41f11-121">Authorization</span></span>|<span data-ttu-id="41f11-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41f11-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41f11-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41f11-123">Accept</span></span>|<span data-ttu-id="41f11-124">application/json</span><span class="sxs-lookup"><span data-stu-id="41f11-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41f11-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41f11-125">Request body</span></span>
<span data-ttu-id="41f11-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41f11-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41f11-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="41f11-127">Response</span></span>
<span data-ttu-id="41f11-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41f11-128">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41f11-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41f11-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="41f11-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41f11-130">Request</span></span>
<span data-ttu-id="41f11-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41f11-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="41f11-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="41f11-132">Response</span></span>
<span data-ttu-id="41f11-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41f11-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
      "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



