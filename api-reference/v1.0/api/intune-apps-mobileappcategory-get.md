---
title: Get mobileAppCategory
description: Ler propriedades e relações do objeto mobileAppCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b6d42ebbe99f02d12f60bf4fc50d27ac8fd3e648
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066961"
---
# <a name="get-mobileappcategory"></a><span data-ttu-id="87a50-103">Get mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="87a50-103">Get mobileAppCategory</span></span>

<span data-ttu-id="87a50-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87a50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87a50-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87a50-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87a50-106">Ler propriedades e relações do objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="87a50-106">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87a50-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87a50-107">Prerequisites</span></span>
<span data-ttu-id="87a50-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87a50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87a50-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87a50-110">Permission type</span></span>|<span data-ttu-id="87a50-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87a50-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87a50-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87a50-112">Delegated (work or school account)</span></span>|<span data-ttu-id="87a50-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="87a50-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="87a50-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87a50-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87a50-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87a50-115">Not supported.</span></span>|
|<span data-ttu-id="87a50-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87a50-116">Application</span></span>|<span data-ttu-id="87a50-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87a50-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87a50-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87a50-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87a50-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87a50-119">Optional query parameters</span></span>
<span data-ttu-id="87a50-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87a50-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87a50-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87a50-121">Request headers</span></span>
|<span data-ttu-id="87a50-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87a50-122">Header</span></span>|<span data-ttu-id="87a50-123">Valor</span><span class="sxs-lookup"><span data-stu-id="87a50-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87a50-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="87a50-124">Authorization</span></span>|<span data-ttu-id="87a50-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87a50-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87a50-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87a50-126">Accept</span></span>|<span data-ttu-id="87a50-127">application/json</span><span class="sxs-lookup"><span data-stu-id="87a50-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87a50-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87a50-128">Request body</span></span>
<span data-ttu-id="87a50-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87a50-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87a50-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="87a50-130">Response</span></span>
<span data-ttu-id="87a50-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87a50-131">If successful, this method returns a `200 OK` response code and [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87a50-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87a50-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="87a50-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87a50-133">Request</span></span>
<span data-ttu-id="87a50-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87a50-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
```

### <a name="response"></a><span data-ttu-id="87a50-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="87a50-135">Response</span></span>
<span data-ttu-id="87a50-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87a50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 239

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppCategory",
    "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```









