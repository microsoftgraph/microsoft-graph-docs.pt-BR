---
title: Listar mobileAppCategories
description: Listar propriedades e as relações dos objetos mobileAppCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 906b7fa291a8f4f663ced05d546cc76f9931f8f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947320"
---
# <a name="list-mobileappcategories"></a><span data-ttu-id="581d3-103">Listar mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="581d3-103">List mobileAppCategories</span></span>

> <span data-ttu-id="581d3-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="581d3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="581d3-105">Listar propriedades e as relações dos objetos [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="581d3-105">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="581d3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="581d3-106">Prerequisites</span></span>
<span data-ttu-id="581d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="581d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="581d3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="581d3-109">Permission type</span></span>|<span data-ttu-id="581d3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="581d3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="581d3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="581d3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="581d3-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="581d3-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="581d3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="581d3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="581d3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="581d3-114">Not supported.</span></span>|
|<span data-ttu-id="581d3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="581d3-115">Application</span></span>|<span data-ttu-id="581d3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="581d3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="581d3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="581d3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="581d3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="581d3-118">Request headers</span></span>
|<span data-ttu-id="581d3-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="581d3-119">Header</span></span>|<span data-ttu-id="581d3-120">Valor</span><span class="sxs-lookup"><span data-stu-id="581d3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="581d3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="581d3-121">Authorization</span></span>|<span data-ttu-id="581d3-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="581d3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="581d3-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="581d3-123">Accept</span></span>|<span data-ttu-id="581d3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="581d3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="581d3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="581d3-125">Request body</span></span>
<span data-ttu-id="581d3-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="581d3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="581d3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="581d3-127">Response</span></span>
<span data-ttu-id="581d3-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="581d3-128">If successful, this method returns a `200 OK` response code and a collection of [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="581d3-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="581d3-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="581d3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="581d3-130">Request</span></span>
<span data-ttu-id="581d3-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="581d3-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories
```

### <a name="response"></a><span data-ttu-id="581d3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="581d3-132">Response</span></span>
<span data-ttu-id="581d3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="581d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppCategory",
      "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```



