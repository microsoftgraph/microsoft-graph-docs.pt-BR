---
title: Get mobileAppCategory
description: Ler propriedades e relações do objeto mobileAppCategory.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3ef51f39e1844769d7b4342573d52e4a46b05a0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892306"
---
# <a name="get-mobileappcategory"></a><span data-ttu-id="6eb5a-103">Get mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="6eb5a-103">Get mobileAppCategory</span></span>

> <span data-ttu-id="6eb5a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6eb5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6eb5a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6eb5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6eb5a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6eb5a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6eb5a-107">Ler propriedades e relações do objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="6eb5a-107">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6eb5a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6eb5a-108">Prerequisites</span></span>
<span data-ttu-id="6eb5a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6eb5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6eb5a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6eb5a-111">Permission type</span></span>|<span data-ttu-id="6eb5a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6eb5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6eb5a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6eb5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6eb5a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6eb5a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6eb5a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6eb5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6eb5a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6eb5a-116">Not supported.</span></span>|
|<span data-ttu-id="6eb5a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6eb5a-117">Application</span></span>|<span data-ttu-id="6eb5a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6eb5a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6eb5a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6eb5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6eb5a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6eb5a-120">Optional query parameters</span></span>
<span data-ttu-id="6eb5a-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6eb5a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6eb5a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6eb5a-122">Request headers</span></span>
|<span data-ttu-id="6eb5a-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6eb5a-123">Header</span></span>|<span data-ttu-id="6eb5a-124">Valor</span><span class="sxs-lookup"><span data-stu-id="6eb5a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6eb5a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6eb5a-125">Authorization</span></span>|<span data-ttu-id="6eb5a-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6eb5a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6eb5a-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6eb5a-127">Accept</span></span>|<span data-ttu-id="6eb5a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6eb5a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6eb5a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6eb5a-129">Request body</span></span>
<span data-ttu-id="6eb5a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6eb5a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6eb5a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6eb5a-131">Response</span></span>
<span data-ttu-id="6eb5a-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6eb5a-132">If successful, this method returns a `200 OK` response code and [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6eb5a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6eb5a-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="6eb5a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6eb5a-134">Request</span></span>
<span data-ttu-id="6eb5a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6eb5a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
```

### <a name="response"></a><span data-ttu-id="6eb5a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6eb5a-136">Response</span></span>
<span data-ttu-id="6eb5a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6eb5a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





