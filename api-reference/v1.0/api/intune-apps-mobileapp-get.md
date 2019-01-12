---
title: Acessar mobileApp
description: Leia as propriedades e as relações do objeto mobileApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ea815b3d69085c085e505e0aee8cabec26f41b95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990233"
---
# <a name="get-mobileapp"></a><span data-ttu-id="6a04d-103">Acessar mobileApp</span><span class="sxs-lookup"><span data-stu-id="6a04d-103">Get mobileApp</span></span>

> <span data-ttu-id="6a04d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6a04d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a04d-105">Leia as propriedades e as relações do objeto [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a04d-105">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6a04d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a04d-106">Prerequisites</span></span>
<span data-ttu-id="6a04d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a04d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a04d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a04d-109">Permission type</span></span>|<span data-ttu-id="6a04d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a04d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a04d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a04d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6a04d-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a04d-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6a04d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a04d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a04d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a04d-114">Not supported.</span></span>|
|<span data-ttu-id="6a04d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a04d-115">Application</span></span>|<span data-ttu-id="6a04d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a04d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a04d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a04d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a04d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a04d-118">Optional query parameters</span></span>
<span data-ttu-id="6a04d-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a04d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6a04d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a04d-120">Request headers</span></span>
|<span data-ttu-id="6a04d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a04d-121">Header</span></span>|<span data-ttu-id="6a04d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6a04d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a04d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a04d-123">Authorization</span></span>|<span data-ttu-id="6a04d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a04d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a04d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a04d-125">Accept</span></span>|<span data-ttu-id="6a04d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a04d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a04d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a04d-127">Request body</span></span>
<span data-ttu-id="6a04d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a04d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a04d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a04d-129">Response</span></span>
<span data-ttu-id="6a04d-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileApp](../resources/intune-apps-mobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a04d-130">If successful, this method returns a `200 OK` response code and [mobileApp](../resources/intune-apps-mobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a04d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a04d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6a04d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a04d-132">Request</span></span>
<span data-ttu-id="6a04d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a04d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="6a04d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a04d-134">Response</span></span>
<span data-ttu-id="6a04d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a04d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 803

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileApp",
    "id": "0177548a-548a-0177-8a54-77018a547701",
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
    "publishingState": "processing"
  }
}
```



