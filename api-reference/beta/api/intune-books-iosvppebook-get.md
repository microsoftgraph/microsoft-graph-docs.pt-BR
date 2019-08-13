---
title: Acessar iosVppEBook
description: Leia as propriedades e as relações do objeto iosVppEBook.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fab507bbadd4d9942b386ed8eb15de8c119b4686
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328463"
---
# <a name="get-iosvppebook"></a><span data-ttu-id="23336-103">Acessar iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="23336-103">Get iosVppEBook</span></span>

> <span data-ttu-id="23336-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="23336-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23336-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23336-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23336-106">Leia as propriedades e as relações do objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="23336-106">Read properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23336-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="23336-107">Prerequisites</span></span>
<span data-ttu-id="23336-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23336-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23336-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23336-110">Permission type</span></span>|<span data-ttu-id="23336-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="23336-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23336-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23336-112">Delegated (work or school account)</span></span>|<span data-ttu-id="23336-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="23336-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="23336-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23336-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23336-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23336-115">Not supported.</span></span>|
|<span data-ttu-id="23336-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23336-116">Application</span></span>|<span data-ttu-id="23336-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="23336-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23336-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23336-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23336-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="23336-119">Optional query parameters</span></span>
<span data-ttu-id="23336-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="23336-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23336-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23336-121">Request headers</span></span>
|<span data-ttu-id="23336-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23336-122">Header</span></span>|<span data-ttu-id="23336-123">Valor</span><span class="sxs-lookup"><span data-stu-id="23336-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23336-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="23336-124">Authorization</span></span>|<span data-ttu-id="23336-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23336-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23336-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="23336-126">Accept</span></span>|<span data-ttu-id="23336-127">application/json</span><span class="sxs-lookup"><span data-stu-id="23336-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23336-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23336-128">Request body</span></span>
<span data-ttu-id="23336-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23336-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23336-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="23336-130">Response</span></span>
<span data-ttu-id="23336-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosVppEBook](../resources/intune-books-iosvppebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23336-131">If successful, this method returns a `200 OK` response code and [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23336-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23336-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="23336-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23336-133">Request</span></span>
<span data-ttu-id="23336-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23336-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="23336-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="23336-135">Response</span></span>
<span data-ttu-id="23336-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23336-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1101

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
    "usedLicenseCount": 0,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```






