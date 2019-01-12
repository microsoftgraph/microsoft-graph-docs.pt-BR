---
title: Acessar webApp
description: Leia as propriedades e as relações do objeto webApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f67ab042030ae3c3d54895d9d576f44525322443
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972569"
---
# <a name="get-webapp"></a><span data-ttu-id="a2552-103">Acessar webApp</span><span class="sxs-lookup"><span data-stu-id="a2552-103">Get webApp</span></span>

> <span data-ttu-id="a2552-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a2552-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2552-105">Leia as propriedades e as relações do objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2552-105">Read properties and relationships of the [webApp](../resources/intune-apps-webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2552-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a2552-106">Prerequisites</span></span>
<span data-ttu-id="a2552-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2552-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2552-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2552-109">Permission type</span></span>|<span data-ttu-id="a2552-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a2552-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2552-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2552-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a2552-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2552-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a2552-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2552-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2552-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2552-114">Not supported.</span></span>|
|<span data-ttu-id="a2552-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2552-115">Application</span></span>|<span data-ttu-id="a2552-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2552-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2552-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2552-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2552-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a2552-118">Optional query parameters</span></span>
<span data-ttu-id="a2552-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a2552-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a2552-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2552-120">Request headers</span></span>
|<span data-ttu-id="a2552-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2552-121">Header</span></span>|<span data-ttu-id="a2552-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a2552-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2552-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2552-123">Authorization</span></span>|<span data-ttu-id="a2552-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2552-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2552-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a2552-125">Accept</span></span>|<span data-ttu-id="a2552-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2552-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2552-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2552-127">Request body</span></span>
<span data-ttu-id="a2552-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2552-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2552-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2552-129">Response</span></span>
<span data-ttu-id="a2552-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [webApp](../resources/intune-apps-webapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2552-130">If successful, this method returns a `200 OK` response code and [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2552-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2552-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2552-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2552-132">Request</span></span>
<span data-ttu-id="a2552-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2552-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="a2552-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2552-134">Response</span></span>
<span data-ttu-id="a2552-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2552-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 878

{
  "value": {
    "@odata.type": "#microsoft.graph.webApp",
    "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "publishingState": "processing",
    "appUrl": "https://example.com/appUrl/",
    "useManagedBrowser": true
  }
}
```



