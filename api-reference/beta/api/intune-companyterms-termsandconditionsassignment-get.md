---
title: Obter termsAndConditionsAssignment
description: Ler propriedades e relações do objeto termsAndConditionsAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf22fd09505991234836419c5afb71ab30dfc3db
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156641"
---
# <a name="get-termsandconditionsassignment"></a><span data-ttu-id="3a3bb-103">Obter termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="3a3bb-103">Get termsAndConditionsAssignment</span></span>

<span data-ttu-id="3a3bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a3bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a3bb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a3bb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a3bb-107">Ler propriedades e relações do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3a3bb-107">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a3bb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3a3bb-108">Prerequisites</span></span>
<span data-ttu-id="3a3bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a3bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a3bb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a3bb-111">Permission type</span></span>|<span data-ttu-id="3a3bb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3a3bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a3bb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a3bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a3bb-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a3bb-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3a3bb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a3bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a3bb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-116">Not supported.</span></span>|
|<span data-ttu-id="3a3bb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a3bb-117">Application</span></span>|<span data-ttu-id="3a3bb-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a3bb-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a3bb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a3bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a3bb-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3a3bb-120">Optional query parameters</span></span>
<span data-ttu-id="3a3bb-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a3bb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a3bb-122">Request headers</span></span>
|<span data-ttu-id="3a3bb-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a3bb-123">Header</span></span>|<span data-ttu-id="3a3bb-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3a3bb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a3bb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a3bb-125">Authorization</span></span>|<span data-ttu-id="3a3bb-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a3bb-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3a3bb-127">Accept</span></span>|<span data-ttu-id="3a3bb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3a3bb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a3bb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a3bb-129">Request body</span></span>
<span data-ttu-id="3a3bb-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a3bb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a3bb-131">Response</span></span>
<span data-ttu-id="3a3bb-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-132">If successful, this method returns a `200 OK` response code and [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a3bb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a3bb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a3bb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a3bb-134">Request</span></span>
<span data-ttu-id="3a3bb-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="3a3bb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a3bb-136">Response</span></span>
<span data-ttu-id="3a3bb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
    "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
    "target": {
      "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include",
      "collectionId": "Collection Id value"
    }
  }
}
```




