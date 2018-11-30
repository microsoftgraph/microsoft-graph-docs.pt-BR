---
title: Acessar mobileAppContentFile
description: Leia as propriedades e as relações do objeto mobileAppContentFile.
ms.openlocfilehash: f71aceb03ba42106357604a382e07dfe91b3484a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005395"
---
# <a name="get-mobileappcontentfile"></a><span data-ttu-id="72de2-103">Acessar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="72de2-103">Get mobileAppContentFile</span></span>

> <span data-ttu-id="72de2-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="72de2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72de2-105">Leia as propriedades e as relações do objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="72de2-105">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="72de2-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72de2-106">Prerequisites</span></span>
<span data-ttu-id="72de2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72de2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72de2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72de2-109">Permission type</span></span>|<span data-ttu-id="72de2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="72de2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72de2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72de2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="72de2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="72de2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="72de2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72de2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72de2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72de2-114">Not supported.</span></span>|
|<span data-ttu-id="72de2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72de2-115">Application</span></span>|<span data-ttu-id="72de2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72de2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72de2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72de2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72de2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="72de2-118">Optional query parameters</span></span>
<span data-ttu-id="72de2-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="72de2-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="72de2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72de2-120">Request headers</span></span>
|<span data-ttu-id="72de2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72de2-121">Header</span></span>|<span data-ttu-id="72de2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="72de2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72de2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="72de2-123">Authorization</span></span>|<span data-ttu-id="72de2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72de2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72de2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="72de2-125">Accept</span></span>|<span data-ttu-id="72de2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72de2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72de2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72de2-127">Request body</span></span>
<span data-ttu-id="72de2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72de2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72de2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="72de2-129">Response</span></span>
<span data-ttu-id="72de2-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72de2-130">If successful, this method returns a `200 OK` response code and [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72de2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72de2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="72de2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72de2-132">Request</span></span>
<span data-ttu-id="72de2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72de2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

### <a name="response"></a><span data-ttu-id="72de2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="72de2-134">Response</span></span>
<span data-ttu-id="72de2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72de2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 491

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppContentFile",
    "azureStorageUri": "Azure Storage Uri value",
    "isCommitted": true,
    "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "name": "Name value",
    "size": 4,
    "sizeEncrypted": 13,
    "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
    "manifest": "bWFuaWZlc3Q=",
    "uploadState": "transientError"
  }
}
```



