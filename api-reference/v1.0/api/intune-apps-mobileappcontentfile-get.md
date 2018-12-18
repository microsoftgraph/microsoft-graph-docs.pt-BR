---
title: Acessar mobileAppContentFile
description: Leia as propriedades e as relações do objeto mobileAppContentFile.
author: tfitzmac
ms.openlocfilehash: 0494b834c6817c08eac750859138f673a793d02a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301089"
---
# <a name="get-mobileappcontentfile"></a><span data-ttu-id="34542-103">Acessar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="34542-103">Get mobileAppContentFile</span></span>

> <span data-ttu-id="34542-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="34542-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34542-105">Leia as propriedades e as relações do objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="34542-105">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="34542-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34542-106">Prerequisites</span></span>
<span data-ttu-id="34542-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34542-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34542-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34542-109">Permission type</span></span>|<span data-ttu-id="34542-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34542-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34542-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34542-111">Delegated (work or school account)</span></span>|<span data-ttu-id="34542-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="34542-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="34542-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34542-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34542-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34542-114">Not supported.</span></span>|
|<span data-ttu-id="34542-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34542-115">Application</span></span>|<span data-ttu-id="34542-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34542-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34542-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34542-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34542-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="34542-118">Optional query parameters</span></span>
<span data-ttu-id="34542-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="34542-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="34542-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34542-120">Request headers</span></span>
|<span data-ttu-id="34542-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34542-121">Header</span></span>|<span data-ttu-id="34542-122">Valor</span><span class="sxs-lookup"><span data-stu-id="34542-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34542-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="34542-123">Authorization</span></span>|<span data-ttu-id="34542-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34542-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34542-125">Accept</span><span class="sxs-lookup"><span data-stu-id="34542-125">Accept</span></span>|<span data-ttu-id="34542-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34542-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34542-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34542-127">Request body</span></span>
<span data-ttu-id="34542-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34542-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34542-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="34542-129">Response</span></span>
<span data-ttu-id="34542-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34542-130">If successful, this method returns a `200 OK` response code and [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34542-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34542-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="34542-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34542-132">Request</span></span>
<span data-ttu-id="34542-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34542-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

### <a name="response"></a><span data-ttu-id="34542-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="34542-134">Response</span></span>
<span data-ttu-id="34542-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34542-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



