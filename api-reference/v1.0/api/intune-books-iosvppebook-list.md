---
title: Listar iosVppEBooks
description: Lista propriedades e relações dos objetos iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2f21ed4efab8548ebb972d441639256eb914029d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256795"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="0a1bd-103">Listar iosVppEBooks</span><span class="sxs-lookup"><span data-stu-id="0a1bd-103">List iosVppEBooks</span></span>

> <span data-ttu-id="0a1bd-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a1bd-105">Listar propriedades e relações dos objetos [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="0a1bd-105">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a1bd-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a1bd-106">Prerequisites</span></span>
<span data-ttu-id="0a1bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0a1bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0a1bd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a1bd-109">Permission type</span></span>|<span data-ttu-id="0a1bd-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0a1bd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a1bd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a1bd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0a1bd-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a1bd-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0a1bd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a1bd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a1bd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-114">Not supported.</span></span>|
|<span data-ttu-id="0a1bd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a1bd-115">Application</span></span>|<span data-ttu-id="0a1bd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a1bd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a1bd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="0a1bd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1bd-118">Request headers</span></span>
|<span data-ttu-id="0a1bd-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a1bd-119">Header</span></span>|<span data-ttu-id="0a1bd-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0a1bd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a1bd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a1bd-121">Authorization</span></span>|<span data-ttu-id="0a1bd-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a1bd-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0a1bd-123">Accept</span></span>|<span data-ttu-id="0a1bd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0a1bd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a1bd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1bd-125">Request body</span></span>
<span data-ttu-id="0a1bd-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a1bd-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a1bd-127">Response</span></span>
<span data-ttu-id="0a1bd-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosVppEBook](../resources/intune-books-iosvppebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-128">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a1bd-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a1bd-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a1bd-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1bd-130">Request</span></span>
<span data-ttu-id="0a1bd-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="0a1bd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a1bd-132">Response</span></span>
<span data-ttu-id="0a1bd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1097

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppEBook",
      "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
      "largeCover": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "informationUrl": "https://example.com/informationUrl/",
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
      "appleId": "Apple Id value",
      "vppOrganizationName": "Vpp Organization Name value",
      "genres": [
        "Genres value"
      ],
      "language": "Language value",
      "seller": "Seller value",
      "totalLicenseCount": 1,
      "usedLicenseCount": 0
    }
  ]
}
```



