---
title: Listar mobileLobApps
description: Listar propriedades e relações dos objetos mobileLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 417c3bfcb1d5d316712654a647ced345dcf00899
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758740"
---
# <a name="list-mobilelobapps"></a><span data-ttu-id="dfe61-103">Listar mobileLobApps</span><span class="sxs-lookup"><span data-stu-id="dfe61-103">List mobileLobApps</span></span>

<span data-ttu-id="dfe61-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfe61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dfe61-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dfe61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfe61-106">Listar propriedades e relações dos objetos [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfe61-106">List properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfe61-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dfe61-107">Prerequisites</span></span>
<span data-ttu-id="dfe61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfe61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfe61-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfe61-110">Permission type</span></span>|<span data-ttu-id="dfe61-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfe61-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfe61-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfe61-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dfe61-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfe61-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dfe61-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfe61-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfe61-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfe61-115">Not supported.</span></span>|
|<span data-ttu-id="dfe61-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfe61-116">Application</span></span>|<span data-ttu-id="dfe61-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfe61-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfe61-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfe61-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="dfe61-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfe61-119">Request headers</span></span>
|<span data-ttu-id="dfe61-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dfe61-120">Header</span></span>|<span data-ttu-id="dfe61-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dfe61-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfe61-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfe61-122">Authorization</span></span>|<span data-ttu-id="dfe61-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfe61-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfe61-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dfe61-124">Accept</span></span>|<span data-ttu-id="dfe61-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dfe61-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfe61-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfe61-126">Request body</span></span>
<span data-ttu-id="dfe61-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfe61-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfe61-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfe61-128">Response</span></span>
<span data-ttu-id="dfe61-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileLobApp](../resources/intune-apps-mobilelobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfe61-129">If successful, this method returns a `200 OK` response code and a collection of [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfe61-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfe61-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfe61-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfe61-131">Request</span></span>
<span data-ttu-id="dfe61-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfe61-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="dfe61-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfe61-133">Response</span></span>
<span data-ttu-id="dfe61-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfe61-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 983

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileLobApp",
      "id": "2fc11935-1935-2fc1-3519-c12f3519c12f",
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
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4
    }
  ]
}
```




