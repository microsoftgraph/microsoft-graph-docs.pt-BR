---
title: Listar iosVppEBooks
description: Listar propriedades e relações dos objetos iosVppEBook.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c447954990464b504ae08f09f285b9ccc9e682ef
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37171285"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="27bfc-103">Listar iosVppEBooks</span><span class="sxs-lookup"><span data-stu-id="27bfc-103">List iosVppEBooks</span></span>

> <span data-ttu-id="27bfc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27bfc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27bfc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27bfc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27bfc-106">Listar propriedades e relações dos objetos [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="27bfc-106">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27bfc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27bfc-107">Prerequisites</span></span>
<span data-ttu-id="27bfc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27bfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27bfc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27bfc-110">Permission type</span></span>|<span data-ttu-id="27bfc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27bfc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27bfc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27bfc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27bfc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="27bfc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="27bfc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27bfc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27bfc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27bfc-115">Not supported.</span></span>|
|<span data-ttu-id="27bfc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27bfc-116">Application</span></span>|<span data-ttu-id="27bfc-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="27bfc-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27bfc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27bfc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="27bfc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27bfc-119">Request headers</span></span>
|<span data-ttu-id="27bfc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27bfc-120">Header</span></span>|<span data-ttu-id="27bfc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="27bfc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27bfc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="27bfc-122">Authorization</span></span>|<span data-ttu-id="27bfc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27bfc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27bfc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27bfc-124">Accept</span></span>|<span data-ttu-id="27bfc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27bfc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27bfc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27bfc-126">Request body</span></span>
<span data-ttu-id="27bfc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27bfc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27bfc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="27bfc-128">Response</span></span>
<span data-ttu-id="27bfc-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosVppEBook](../resources/intune-books-iosvppebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27bfc-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27bfc-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27bfc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="27bfc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27bfc-131">Request</span></span>
<span data-ttu-id="27bfc-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27bfc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="27bfc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="27bfc-133">Response</span></span>
<span data-ttu-id="27bfc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27bfc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1171

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
      "usedLicenseCount": 0,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




