---
title: Listar iosVppEBooks
description: Listar propriedades e relações dos objetos iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b5aa595063c3fdaf0769edac1f574610daa23da
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960136"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="8c531-103">Listar iosVppEBooks</span><span class="sxs-lookup"><span data-stu-id="8c531-103">List iosVppEBooks</span></span>

> <span data-ttu-id="8c531-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c531-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c531-105">Listar propriedades e relações dos objetos [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="8c531-105">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c531-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c531-106">Prerequisites</span></span>
<span data-ttu-id="8c531-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c531-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c531-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c531-109">Permission type</span></span>|<span data-ttu-id="8c531-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8c531-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c531-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c531-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c531-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c531-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8c531-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c531-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c531-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c531-114">Not supported.</span></span>|
|<span data-ttu-id="8c531-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c531-115">Application</span></span>|<span data-ttu-id="8c531-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c531-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c531-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c531-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="8c531-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c531-118">Request headers</span></span>
|<span data-ttu-id="8c531-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c531-119">Header</span></span>|<span data-ttu-id="8c531-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8c531-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c531-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c531-121">Authorization</span></span>|<span data-ttu-id="8c531-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c531-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c531-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8c531-123">Accept</span></span>|<span data-ttu-id="8c531-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8c531-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c531-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c531-125">Request body</span></span>
<span data-ttu-id="8c531-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8c531-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c531-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c531-127">Response</span></span>
<span data-ttu-id="8c531-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosVppEBook](../resources/intune-books-iosvppebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c531-128">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c531-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c531-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c531-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c531-130">Request</span></span>
<span data-ttu-id="8c531-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c531-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="8c531-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c531-132">Response</span></span>
<span data-ttu-id="8c531-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c531-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



