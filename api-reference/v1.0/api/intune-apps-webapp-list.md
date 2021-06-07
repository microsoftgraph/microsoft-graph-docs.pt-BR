---
title: Listar webApps
description: Listar propriedades e relações dos objetos webApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 34845cc9557f7039e0f5c3e049158bbbb452ac4b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757294"
---
# <a name="list-webapps"></a><span data-ttu-id="66cc5-103">Listar webApps</span><span class="sxs-lookup"><span data-stu-id="66cc5-103">List webApps</span></span>

<span data-ttu-id="66cc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66cc5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66cc5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="66cc5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66cc5-106">Listar propriedades e relações dos objetos [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="66cc5-106">List properties and relationships of the [webApp](../resources/intune-apps-webapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66cc5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="66cc5-107">Prerequisites</span></span>
<span data-ttu-id="66cc5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66cc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66cc5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66cc5-110">Permission type</span></span>|<span data-ttu-id="66cc5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66cc5-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66cc5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66cc5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66cc5-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66cc5-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66cc5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66cc5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66cc5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66cc5-115">Not supported.</span></span>|
|<span data-ttu-id="66cc5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66cc5-116">Application</span></span>|<span data-ttu-id="66cc5-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66cc5-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66cc5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66cc5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="66cc5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66cc5-119">Request headers</span></span>
|<span data-ttu-id="66cc5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="66cc5-120">Header</span></span>|<span data-ttu-id="66cc5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="66cc5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66cc5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="66cc5-122">Authorization</span></span>|<span data-ttu-id="66cc5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66cc5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66cc5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="66cc5-124">Accept</span></span>|<span data-ttu-id="66cc5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66cc5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66cc5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66cc5-126">Request body</span></span>
<span data-ttu-id="66cc5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="66cc5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66cc5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="66cc5-128">Response</span></span>
<span data-ttu-id="66cc5-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [webApp](../resources/intune-apps-webapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66cc5-129">If successful, this method returns a `200 OK` response code and a collection of [webApp](../resources/intune-apps-webapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66cc5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66cc5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="66cc5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66cc5-131">Request</span></span>
<span data-ttu-id="66cc5-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66cc5-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="66cc5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="66cc5-133">Response</span></span>
<span data-ttu-id="66cc5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66cc5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 934

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.webApp",
      "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
      "appUrl": "https://example.com/appUrl/",
      "useManagedBrowser": true
    }
  ]
}
```




