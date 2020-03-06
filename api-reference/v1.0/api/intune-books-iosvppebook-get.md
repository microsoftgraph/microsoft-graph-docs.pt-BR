---
title: Acessar iosVppEBook
description: Leia as propriedades e as relações do objeto iosVppEBook.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e3f9cc3db0ef02a4cd2a113709029f07063caca6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515648"
---
# <a name="get-iosvppebook"></a><span data-ttu-id="8cffc-103">Acessar iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="8cffc-103">Get iosVppEBook</span></span>

<span data-ttu-id="8cffc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cffc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cffc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cffc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cffc-106">Leia as propriedades e as relações do objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="8cffc-106">Read properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cffc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8cffc-107">Prerequisites</span></span>
<span data-ttu-id="8cffc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cffc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cffc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cffc-110">Permission type</span></span>|<span data-ttu-id="8cffc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8cffc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cffc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cffc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8cffc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cffc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8cffc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cffc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cffc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cffc-115">Not supported.</span></span>|
|<span data-ttu-id="8cffc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cffc-116">Application</span></span>|<span data-ttu-id="8cffc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cffc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cffc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cffc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8cffc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8cffc-119">Optional query parameters</span></span>
<span data-ttu-id="8cffc-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8cffc-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8cffc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cffc-121">Request headers</span></span>
|<span data-ttu-id="8cffc-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cffc-122">Header</span></span>|<span data-ttu-id="8cffc-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8cffc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cffc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cffc-124">Authorization</span></span>|<span data-ttu-id="8cffc-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cffc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cffc-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8cffc-126">Accept</span></span>|<span data-ttu-id="8cffc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8cffc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cffc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cffc-128">Request body</span></span>
<span data-ttu-id="8cffc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8cffc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cffc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cffc-130">Response</span></span>
<span data-ttu-id="8cffc-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosVppEBook](../resources/intune-books-iosvppebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cffc-131">If successful, this method returns a `200 OK` response code and [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cffc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cffc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cffc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cffc-133">Request</span></span>
<span data-ttu-id="8cffc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cffc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="8cffc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cffc-135">Response</span></span>
<span data-ttu-id="8cffc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cffc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1033

{
  "value": {
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
}
```




