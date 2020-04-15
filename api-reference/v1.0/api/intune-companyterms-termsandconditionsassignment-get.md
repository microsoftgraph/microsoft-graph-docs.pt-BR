---
title: Obter termsAndConditionsAssignment
description: Ler propriedades e relações do objeto termsAndConditionsAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4231579e4e98423eb399971e92efa6fd812a3596
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442122"
---
# <a name="get-termsandconditionsassignment"></a><span data-ttu-id="2f862-103">Obter termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2f862-103">Get termsAndConditionsAssignment</span></span>

<span data-ttu-id="2f862-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f862-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f862-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f862-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f862-106">Ler propriedades e relações do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2f862-106">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f862-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f862-107">Prerequisites</span></span>
<span data-ttu-id="2f862-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f862-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f862-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f862-110">Permission type</span></span>|<span data-ttu-id="2f862-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f862-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f862-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f862-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f862-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f862-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2f862-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f862-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f862-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f862-115">Not supported.</span></span>|
|<span data-ttu-id="2f862-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f862-116">Application</span></span>|<span data-ttu-id="2f862-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f862-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f862-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f862-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f862-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2f862-119">Optional query parameters</span></span>
<span data-ttu-id="2f862-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2f862-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f862-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f862-121">Request headers</span></span>
|<span data-ttu-id="2f862-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f862-122">Header</span></span>|<span data-ttu-id="2f862-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2f862-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f862-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f862-124">Authorization</span></span>|<span data-ttu-id="2f862-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f862-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f862-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f862-126">Accept</span></span>|<span data-ttu-id="2f862-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2f862-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f862-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f862-128">Request body</span></span>
<span data-ttu-id="2f862-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f862-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f862-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f862-130">Response</span></span>
<span data-ttu-id="2f862-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f862-131">If successful, this method returns a `200 OK` response code and [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f862-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f862-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f862-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f862-133">Request</span></span>
<span data-ttu-id="2f862-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f862-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="2f862-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f862-135">Response</span></span>
<span data-ttu-id="2f862-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f862-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 246

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
    "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```






