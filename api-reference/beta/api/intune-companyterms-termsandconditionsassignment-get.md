---
title: Obter termsAndConditionsAssignment
description: Ler propriedades e relações do objeto termsAndConditionsAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b3eb9d15a2c32c6f3b784cbf411a2f8e8c53415b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793168"
---
# <a name="get-termsandconditionsassignment"></a><span data-ttu-id="d93ad-103">Obter termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d93ad-103">Get termsAndConditionsAssignment</span></span>

<span data-ttu-id="d93ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d93ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d93ad-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d93ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d93ad-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d93ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d93ad-107">Ler propriedades e relações do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d93ad-107">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d93ad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d93ad-108">Prerequisites</span></span>
<span data-ttu-id="d93ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d93ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d93ad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d93ad-111">Permission type</span></span>|<span data-ttu-id="d93ad-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d93ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d93ad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d93ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d93ad-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d93ad-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d93ad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d93ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d93ad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d93ad-116">Not supported.</span></span>|
|<span data-ttu-id="d93ad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d93ad-117">Application</span></span>|<span data-ttu-id="d93ad-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d93ad-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d93ad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d93ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d93ad-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d93ad-120">Optional query parameters</span></span>
<span data-ttu-id="d93ad-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d93ad-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d93ad-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d93ad-122">Request headers</span></span>
|<span data-ttu-id="d93ad-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d93ad-123">Header</span></span>|<span data-ttu-id="d93ad-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d93ad-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d93ad-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d93ad-125">Authorization</span></span>|<span data-ttu-id="d93ad-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d93ad-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d93ad-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d93ad-127">Accept</span></span>|<span data-ttu-id="d93ad-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d93ad-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d93ad-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d93ad-129">Request body</span></span>
<span data-ttu-id="d93ad-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d93ad-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d93ad-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d93ad-131">Response</span></span>
<span data-ttu-id="d93ad-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d93ad-132">If successful, this method returns a `200 OK` response code and [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d93ad-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d93ad-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d93ad-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d93ad-134">Request</span></span>
<span data-ttu-id="d93ad-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d93ad-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="d93ad-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d93ad-136">Response</span></span>
<span data-ttu-id="d93ad-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d93ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 405

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
    "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
    "target": {
      "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    }
  }
}
```



