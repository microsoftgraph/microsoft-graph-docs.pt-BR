---
title: Acessar mobileLobApp
description: Leia as propriedades e as relações do objeto mobileLobApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 54a7337fc83ed4d9cb715def2e5404c7208ac27b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855493"
---
# <a name="get-mobilelobapp"></a><span data-ttu-id="a5d9d-103">Acessar mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="a5d9d-103">Get mobileLobApp</span></span>

> <span data-ttu-id="a5d9d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a5d9d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5d9d-105">Leia as propriedades e as relações do objeto [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a5d9d-105">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a5d9d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a5d9d-106">Prerequisites</span></span>
<span data-ttu-id="a5d9d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5d9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5d9d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5d9d-109">Permission type</span></span>|<span data-ttu-id="a5d9d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a5d9d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5d9d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5d9d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a5d9d-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5d9d-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a5d9d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5d9d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5d9d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5d9d-114">Not supported.</span></span>|
|<span data-ttu-id="a5d9d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5d9d-115">Application</span></span>|<span data-ttu-id="a5d9d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5d9d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5d9d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5d9d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5d9d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a5d9d-118">Optional query parameters</span></span>
<span data-ttu-id="a5d9d-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a5d9d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a5d9d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5d9d-120">Request headers</span></span>
|<span data-ttu-id="a5d9d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5d9d-121">Header</span></span>|<span data-ttu-id="a5d9d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a5d9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5d9d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5d9d-123">Authorization</span></span>|<span data-ttu-id="a5d9d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5d9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5d9d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a5d9d-125">Accept</span></span>|<span data-ttu-id="a5d9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5d9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5d9d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5d9d-127">Request body</span></span>
<span data-ttu-id="a5d9d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5d9d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5d9d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5d9d-129">Response</span></span>
<span data-ttu-id="a5d9d-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileLobApp](../resources/intune-apps-mobilelobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5d9d-130">If successful, this method returns a `200 OK` response code and [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5d9d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5d9d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5d9d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5d9d-132">Request</span></span>
<span data-ttu-id="a5d9d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5d9d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="a5d9d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5d9d-134">Response</span></span>
<span data-ttu-id="a5d9d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5d9d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 925

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileLobApp",
    "id": "2fc11935-1935-2fc1-3519-c12f3519c12f",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4
  }
}
```



