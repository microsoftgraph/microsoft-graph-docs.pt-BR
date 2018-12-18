---
title: Listar mobileApps
description: Listar propriedades e relações dos objetos mobileApp.
author: tfitzmac
ms.openlocfilehash: aafc9bfa6f602dd462bc8cfb95c83bce9324e655
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349116"
---
# <a name="list-mobileapps"></a><span data-ttu-id="77062-103">Listar mobileApps</span><span class="sxs-lookup"><span data-stu-id="77062-103">List mobileApps</span></span>

> <span data-ttu-id="77062-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="77062-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77062-105">Listar propriedades e relações dos objetos [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="77062-105">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="77062-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77062-106">Prerequisites</span></span>
<span data-ttu-id="77062-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77062-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77062-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77062-109">Permission type</span></span>|<span data-ttu-id="77062-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="77062-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77062-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77062-111">Delegated (work or school account)</span></span>|<span data-ttu-id="77062-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="77062-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="77062-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77062-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77062-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77062-114">Not supported.</span></span>|
|<span data-ttu-id="77062-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77062-115">Application</span></span>|<span data-ttu-id="77062-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77062-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77062-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77062-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="77062-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77062-118">Request headers</span></span>
|<span data-ttu-id="77062-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77062-119">Header</span></span>|<span data-ttu-id="77062-120">Valor</span><span class="sxs-lookup"><span data-stu-id="77062-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77062-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="77062-121">Authorization</span></span>|<span data-ttu-id="77062-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77062-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77062-123">Accept</span><span class="sxs-lookup"><span data-stu-id="77062-123">Accept</span></span>|<span data-ttu-id="77062-124">application/json</span><span class="sxs-lookup"><span data-stu-id="77062-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77062-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77062-125">Request body</span></span>
<span data-ttu-id="77062-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="77062-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77062-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="77062-127">Response</span></span>
<span data-ttu-id="77062-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileApp](../resources/intune-apps-mobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77062-128">If successful, this method returns a `200 OK` response code and a collection of [mobileApp](../resources/intune-apps-mobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77062-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77062-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="77062-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77062-130">Request</span></span>
<span data-ttu-id="77062-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77062-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="77062-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="77062-132">Response</span></span>
<span data-ttu-id="77062-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77062-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
  "value": [
    {
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
  ]
}
```



