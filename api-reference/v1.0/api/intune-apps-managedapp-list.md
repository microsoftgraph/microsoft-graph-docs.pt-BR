---
title: Listar managedApps
description: Listar propriedades e relações dos objetos managedApp.
ms.openlocfilehash: 5c7994864ac5351bfd5533e989a50837d11c17ec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007164"
---
# <a name="list-managedapps"></a><span data-ttu-id="5c137-103">Listar managedApps</span><span class="sxs-lookup"><span data-stu-id="5c137-103">List managedApps</span></span>

> <span data-ttu-id="5c137-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5c137-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c137-105">Listar propriedades e relações dos objetos [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c137-105">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c137-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c137-106">Prerequisites</span></span>
<span data-ttu-id="5c137-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c137-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c137-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c137-109">Permission type</span></span>|<span data-ttu-id="5c137-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c137-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c137-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c137-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c137-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c137-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5c137-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c137-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c137-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c137-114">Not supported.</span></span>|
|<span data-ttu-id="5c137-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c137-115">Application</span></span>|<span data-ttu-id="5c137-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c137-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c137-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c137-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5c137-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c137-118">Request headers</span></span>
|<span data-ttu-id="5c137-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c137-119">Header</span></span>|<span data-ttu-id="5c137-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5c137-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c137-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c137-121">Authorization</span></span>|<span data-ttu-id="5c137-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c137-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c137-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5c137-123">Accept</span></span>|<span data-ttu-id="5c137-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5c137-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c137-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c137-125">Request body</span></span>
<span data-ttu-id="5c137-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c137-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c137-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c137-127">Response</span></span>
<span data-ttu-id="5c137-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedApp](../resources/intune-apps-managedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c137-128">If successful, this method returns a `200 OK` response code and a collection of [managedApp](../resources/intune-apps-managedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c137-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c137-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c137-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c137-130">Request</span></span>
<span data-ttu-id="5c137-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c137-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="5c137-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c137-132">Response</span></span>
<span data-ttu-id="5c137-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c137-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 935

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedApp",
      "id": "f687dd85-dd85-f687-85dd-87f685dd87f6",
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
      "version": "Version value"
    }
  ]
}
```



