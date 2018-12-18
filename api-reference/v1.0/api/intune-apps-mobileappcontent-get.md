---
title: Acessar mobileAppContent
description: Leia as propriedades e as relações do objeto mobileAppContent.
author: tfitzmac
ms.openlocfilehash: ab5c660f4bb5e505e70b7ae71211fcc8c3c69f18
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356522"
---
# <a name="get-mobileappcontent"></a><span data-ttu-id="f0a4b-103">Acessar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="f0a4b-103">Get mobileAppContent</span></span>

> <span data-ttu-id="f0a4b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f0a4b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0a4b-105">Leia as propriedades e as relações do objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="f0a4b-105">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0a4b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f0a4b-106">Prerequisites</span></span>
<span data-ttu-id="f0a4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0a4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0a4b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0a4b-109">Permission type</span></span>|<span data-ttu-id="f0a4b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f0a4b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0a4b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0a4b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f0a4b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0a4b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f0a4b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0a4b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0a4b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0a4b-114">Not supported.</span></span>|
|<span data-ttu-id="f0a4b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0a4b-115">Application</span></span>|<span data-ttu-id="f0a4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0a4b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0a4b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0a4b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0a4b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f0a4b-118">Optional query parameters</span></span>
<span data-ttu-id="f0a4b-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f0a4b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f0a4b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0a4b-120">Request headers</span></span>
|<span data-ttu-id="f0a4b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0a4b-121">Header</span></span>|<span data-ttu-id="f0a4b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f0a4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0a4b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0a4b-123">Authorization</span></span>|<span data-ttu-id="f0a4b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0a4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0a4b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0a4b-125">Accept</span></span>|<span data-ttu-id="f0a4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0a4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0a4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0a4b-127">Request body</span></span>
<span data-ttu-id="f0a4b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0a4b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0a4b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0a4b-129">Response</span></span>
<span data-ttu-id="f0a4b-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0a4b-130">If successful, this method returns a `200 OK` response code and [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0a4b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0a4b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0a4b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0a4b-132">Request</span></span>
<span data-ttu-id="f0a4b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0a4b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="f0a4b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0a4b-134">Response</span></span>
<span data-ttu-id="f0a4b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0a4b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppContent",
    "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
  }
}
```



