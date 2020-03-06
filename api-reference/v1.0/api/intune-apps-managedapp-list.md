---
title: Listar managedApps
description: Listar propriedades e relações dos objetos managedApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8de3163d1ab2910e29c0c2d0cbc8a7adaab29b52
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516367"
---
# <a name="list-managedapps"></a><span data-ttu-id="a3343-103">Listar managedApps</span><span class="sxs-lookup"><span data-stu-id="a3343-103">List managedApps</span></span>

<span data-ttu-id="a3343-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3343-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3343-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a3343-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3343-106">Listar propriedades e relações dos objetos [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3343-106">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3343-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a3343-107">Prerequisites</span></span>
<span data-ttu-id="a3343-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3343-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3343-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3343-110">Permission type</span></span>|<span data-ttu-id="a3343-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a3343-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3343-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3343-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3343-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3343-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a3343-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3343-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3343-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3343-115">Not supported.</span></span>|
|<span data-ttu-id="a3343-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3343-116">Application</span></span>|<span data-ttu-id="a3343-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3343-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3343-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3343-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a3343-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3343-119">Request headers</span></span>
|<span data-ttu-id="a3343-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3343-120">Header</span></span>|<span data-ttu-id="a3343-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a3343-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3343-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3343-122">Authorization</span></span>|<span data-ttu-id="a3343-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3343-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3343-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a3343-124">Accept</span></span>|<span data-ttu-id="a3343-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3343-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3343-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3343-126">Request body</span></span>
<span data-ttu-id="a3343-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3343-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3343-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3343-128">Response</span></span>
<span data-ttu-id="a3343-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedApp](../resources/intune-apps-managedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3343-129">If successful, this method returns a `200 OK` response code and a collection of [managedApp](../resources/intune-apps-managedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3343-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3343-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3343-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3343-131">Request</span></span>
<span data-ttu-id="a3343-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3343-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="a3343-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3343-133">Response</span></span>
<span data-ttu-id="a3343-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3343-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




