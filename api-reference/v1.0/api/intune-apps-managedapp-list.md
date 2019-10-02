---
title: Listar managedApps
description: Listar propriedades e relações dos objetos managedApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 89b9e8263e632b8630330d1b73fec5a282243e3b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358666"
---
# <a name="list-managedapps"></a><span data-ttu-id="bee26-103">Listar managedApps</span><span class="sxs-lookup"><span data-stu-id="bee26-103">List managedApps</span></span>

> <span data-ttu-id="bee26-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bee26-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bee26-105">Listar propriedades e relações dos objetos [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="bee26-105">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bee26-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bee26-106">Prerequisites</span></span>
<span data-ttu-id="bee26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bee26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bee26-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bee26-109">Permission type</span></span>|<span data-ttu-id="bee26-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bee26-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bee26-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bee26-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bee26-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bee26-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bee26-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bee26-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bee26-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bee26-114">Not supported.</span></span>|
|<span data-ttu-id="bee26-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bee26-115">Application</span></span>|<span data-ttu-id="bee26-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bee26-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bee26-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bee26-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bee26-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bee26-118">Request headers</span></span>
|<span data-ttu-id="bee26-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bee26-119">Header</span></span>|<span data-ttu-id="bee26-120">Valor</span><span class="sxs-lookup"><span data-stu-id="bee26-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bee26-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bee26-121">Authorization</span></span>|<span data-ttu-id="bee26-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bee26-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bee26-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bee26-123">Accept</span></span>|<span data-ttu-id="bee26-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bee26-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bee26-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bee26-125">Request body</span></span>
<span data-ttu-id="bee26-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bee26-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bee26-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bee26-127">Response</span></span>
<span data-ttu-id="bee26-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedApp](../resources/intune-apps-managedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bee26-128">If successful, this method returns a `200 OK` response code and a collection of [managedApp](../resources/intune-apps-managedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bee26-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bee26-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="bee26-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bee26-130">Request</span></span>
<span data-ttu-id="bee26-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bee26-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="bee26-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="bee26-132">Response</span></span>
<span data-ttu-id="bee26-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bee26-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




