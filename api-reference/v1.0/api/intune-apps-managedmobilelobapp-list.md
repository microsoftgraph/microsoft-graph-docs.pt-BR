---
title: Listar managedMobileLobApps
description: Listar propriedades e relações dos objetos managedMobileLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2115b07ed07c70822e7fa0f0e1447d8d8559c885
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754144"
---
# <a name="list-managedmobilelobapps"></a><span data-ttu-id="a6662-103">Listar managedMobileLobApps</span><span class="sxs-lookup"><span data-stu-id="a6662-103">List managedMobileLobApps</span></span>

<span data-ttu-id="a6662-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6662-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6662-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6662-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6662-106">Listar propriedades e relações dos objetos [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6662-106">List properties and relationships of the [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6662-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6662-107">Prerequisites</span></span>
<span data-ttu-id="a6662-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6662-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6662-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6662-110">Permission type</span></span>|<span data-ttu-id="a6662-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6662-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6662-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6662-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6662-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6662-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a6662-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6662-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6662-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6662-115">Not supported.</span></span>|
|<span data-ttu-id="a6662-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6662-116">Application</span></span>|<span data-ttu-id="a6662-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6662-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6662-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6662-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a6662-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6662-119">Request headers</span></span>
|<span data-ttu-id="a6662-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6662-120">Header</span></span>|<span data-ttu-id="a6662-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a6662-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6662-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6662-122">Authorization</span></span>|<span data-ttu-id="a6662-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6662-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6662-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6662-124">Accept</span></span>|<span data-ttu-id="a6662-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6662-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6662-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6662-126">Request body</span></span>
<span data-ttu-id="a6662-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6662-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6662-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6662-128">Response</span></span>
<span data-ttu-id="a6662-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6662-129">If successful, this method returns a `200 OK` response code and a collection of [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6662-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6662-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6662-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6662-131">Request</span></span>
<span data-ttu-id="a6662-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6662-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="a6662-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6662-133">Response</span></span>
<span data-ttu-id="a6662-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6662-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1069

{
  "value": [
    {
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
  ]
}
```




