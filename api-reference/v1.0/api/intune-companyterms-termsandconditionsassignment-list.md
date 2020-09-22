---
title: Listar termsAndConditionsAssignments
description: Listar propriedades e relações dos objetos termsAndConditionsAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f78ca6e9e7b5c64233b8f358483e1f685b0bf8ff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972970"
---
# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="a08b1-103">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="a08b1-103">List termsAndConditionsAssignments</span></span>

<span data-ttu-id="a08b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a08b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a08b1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a08b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a08b1-106">Listar propriedades e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a08b1-106">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a08b1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a08b1-107">Prerequisites</span></span>
<span data-ttu-id="a08b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a08b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a08b1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a08b1-110">Permission type</span></span>|<span data-ttu-id="a08b1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a08b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a08b1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a08b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a08b1-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a08b1-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a08b1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a08b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a08b1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a08b1-115">Not supported.</span></span>|
|<span data-ttu-id="a08b1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a08b1-116">Application</span></span>|<span data-ttu-id="a08b1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a08b1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a08b1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a08b1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a08b1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a08b1-119">Request headers</span></span>
|<span data-ttu-id="a08b1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a08b1-120">Header</span></span>|<span data-ttu-id="a08b1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a08b1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a08b1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a08b1-122">Authorization</span></span>|<span data-ttu-id="a08b1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a08b1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a08b1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a08b1-124">Accept</span></span>|<span data-ttu-id="a08b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a08b1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a08b1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a08b1-126">Request body</span></span>
<span data-ttu-id="a08b1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a08b1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a08b1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a08b1-128">Response</span></span>
<span data-ttu-id="a08b1-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a08b1-129">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a08b1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a08b1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a08b1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a08b1-131">Request</span></span>
<span data-ttu-id="a08b1-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a08b1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="a08b1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a08b1-133">Response</span></span>
<span data-ttu-id="a08b1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a08b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









