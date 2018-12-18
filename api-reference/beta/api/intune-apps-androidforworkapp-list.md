---
title: Lista androidForWorkApps
description: Lista as propriedades e os relacionamentos dos objetos androidForWorkApp.
author: tfitzmac
ms.openlocfilehash: 82a1d40e12595c7aec61fbc920aea656547c8d76
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352161"
---
# <a name="list-androidforworkapps"></a><span data-ttu-id="c0c51-103">Lista androidForWorkApps</span><span class="sxs-lookup"><span data-stu-id="c0c51-103">List androidForWorkApps</span></span>

> <span data-ttu-id="c0c51-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c0c51-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0c51-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c0c51-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0c51-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c0c51-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0c51-107">Lista as propriedades e os relacionamentos dos objetos [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="c0c51-107">List properties and relationships of the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0c51-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0c51-108">Prerequisites</span></span>
<span data-ttu-id="c0c51-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0c51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0c51-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0c51-111">Permission type</span></span>|<span data-ttu-id="c0c51-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c0c51-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0c51-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0c51-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0c51-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0c51-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c0c51-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0c51-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0c51-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0c51-116">Not supported.</span></span>|
|<span data-ttu-id="c0c51-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0c51-117">Application</span></span>|<span data-ttu-id="c0c51-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0c51-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0c51-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0c51-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c0c51-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0c51-120">Request headers</span></span>
|<span data-ttu-id="c0c51-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0c51-121">Header</span></span>|<span data-ttu-id="c0c51-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c0c51-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0c51-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0c51-123">Authorization</span></span>|<span data-ttu-id="c0c51-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0c51-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0c51-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c0c51-125">Accept</span></span>|<span data-ttu-id="c0c51-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0c51-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0c51-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0c51-127">Request body</span></span>
<span data-ttu-id="c0c51-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0c51-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0c51-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0c51-129">Response</span></span>
<span data-ttu-id="c0c51-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0c51-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0c51-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0c51-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0c51-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0c51-132">Request</span></span>
<span data-ttu-id="c0c51-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0c51-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="c0c51-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0c51-134">Response</span></span>
<span data-ttu-id="c0c51-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0c51-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1096

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkApp",
      "id": "c5010785-0785-c501-8507-01c5850701c5",
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
      "uploadState": 11,
      "publishingState": "processing",
      "packageId": "Package Id value",
      "appIdentifier": "App Identifier value",
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "appStoreUrl": "https://example.com/appStoreUrl/"
    }
  ]
}
```





