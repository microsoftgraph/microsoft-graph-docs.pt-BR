---
title: Acessar mobileLobApp
description: Leia as propriedades e as relações do objeto mobileLobApp.
ms.openlocfilehash: aa8d69b7b782a3178127c7cd2db93a2c3f42bfb9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005703"
---
# <a name="get-mobilelobapp"></a><span data-ttu-id="a8d09-103">Acessar mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="a8d09-103">Get mobileLobApp</span></span>

> <span data-ttu-id="a8d09-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a8d09-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8d09-105">Leia as propriedades e as relações do objeto [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a8d09-105">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8d09-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8d09-106">Prerequisites</span></span>
<span data-ttu-id="a8d09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8d09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8d09-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8d09-109">Permission type</span></span>|<span data-ttu-id="a8d09-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a8d09-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8d09-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8d09-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a8d09-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8d09-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a8d09-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8d09-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8d09-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8d09-114">Not supported.</span></span>|
|<span data-ttu-id="a8d09-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8d09-115">Application</span></span>|<span data-ttu-id="a8d09-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8d09-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8d09-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8d09-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8d09-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a8d09-118">Optional query parameters</span></span>
<span data-ttu-id="a8d09-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a8d09-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a8d09-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8d09-120">Request headers</span></span>
|<span data-ttu-id="a8d09-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8d09-121">Header</span></span>|<span data-ttu-id="a8d09-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a8d09-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8d09-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8d09-123">Authorization</span></span>|<span data-ttu-id="a8d09-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8d09-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8d09-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a8d09-125">Accept</span></span>|<span data-ttu-id="a8d09-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8d09-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8d09-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8d09-127">Request body</span></span>
<span data-ttu-id="a8d09-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8d09-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8d09-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8d09-129">Response</span></span>
<span data-ttu-id="a8d09-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileLobApp](../resources/intune-apps-mobilelobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8d09-130">If successful, this method returns a `200 OK` response code and [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8d09-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8d09-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8d09-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8d09-132">Request</span></span>
<span data-ttu-id="a8d09-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8d09-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="a8d09-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8d09-134">Response</span></span>
<span data-ttu-id="a8d09-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8d09-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



