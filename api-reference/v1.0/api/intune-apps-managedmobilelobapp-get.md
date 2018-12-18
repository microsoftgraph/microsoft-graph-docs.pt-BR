---
title: Acessar managedMobileLobApp
description: Leia as propriedades e as relações do objeto managedMobileLobApp.
author: tfitzmac
ms.openlocfilehash: b15f4337c8ff5669d50ada9335f1fde7b111f205
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325463"
---
# <a name="get-managedmobilelobapp"></a><span data-ttu-id="86f6e-103">Acessar managedMobileLobApp</span><span class="sxs-lookup"><span data-stu-id="86f6e-103">Get managedMobileLobApp</span></span>

> <span data-ttu-id="86f6e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="86f6e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86f6e-105">Leia as propriedades e as relações do objeto [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="86f6e-105">Read properties and relationships of the [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86f6e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86f6e-106">Prerequisites</span></span>
<span data-ttu-id="86f6e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86f6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86f6e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86f6e-109">Permission type</span></span>|<span data-ttu-id="86f6e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86f6e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86f6e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86f6e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="86f6e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="86f6e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="86f6e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86f6e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86f6e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86f6e-114">Not supported.</span></span>|
|<span data-ttu-id="86f6e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86f6e-115">Application</span></span>|<span data-ttu-id="86f6e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86f6e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86f6e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86f6e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86f6e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="86f6e-118">Optional query parameters</span></span>
<span data-ttu-id="86f6e-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="86f6e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="86f6e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86f6e-120">Request headers</span></span>
|<span data-ttu-id="86f6e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86f6e-121">Header</span></span>|<span data-ttu-id="86f6e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="86f6e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86f6e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="86f6e-123">Authorization</span></span>|<span data-ttu-id="86f6e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86f6e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86f6e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86f6e-125">Accept</span></span>|<span data-ttu-id="86f6e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86f6e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86f6e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86f6e-127">Request body</span></span>
<span data-ttu-id="86f6e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86f6e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86f6e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="86f6e-129">Response</span></span>
<span data-ttu-id="86f6e-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86f6e-130">If successful, this method returns a `200 OK` response code and [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86f6e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86f6e-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="86f6e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86f6e-132">Request</span></span>
<span data-ttu-id="86f6e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86f6e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="86f6e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="86f6e-134">Response</span></span>
<span data-ttu-id="86f6e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86f6e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1007

{
  "value": {
    "@odata.type": "#microsoft.graph.managedMobileLobApp",
    "id": "cded7cc4-7cc4-cded-c47c-edcdc47cedcd",
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
    "appAvailability": "lineOfBusiness",
    "version": "Version value",
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4
  }
}
```



