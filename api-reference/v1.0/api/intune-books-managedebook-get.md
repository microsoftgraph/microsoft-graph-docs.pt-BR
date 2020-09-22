---
title: Acessar managedEBook
description: Leia as propriedades e as relações do objeto managedEBook.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ee0ecc9f3dd0bbc52319beca03e95e5727ed6b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48077881"
---
# <a name="get-managedebook"></a><span data-ttu-id="07076-103">Acessar managedEBook</span><span class="sxs-lookup"><span data-stu-id="07076-103">Get managedEBook</span></span>

<span data-ttu-id="07076-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07076-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07076-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07076-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07076-106">Leia as propriedades e as relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="07076-106">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07076-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07076-107">Prerequisites</span></span>
<span data-ttu-id="07076-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07076-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07076-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07076-110">Permission type</span></span>|<span data-ttu-id="07076-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07076-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07076-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07076-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07076-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="07076-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="07076-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07076-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07076-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07076-115">Not supported.</span></span>|
|<span data-ttu-id="07076-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07076-116">Application</span></span>|<span data-ttu-id="07076-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07076-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07076-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07076-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07076-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="07076-119">Optional query parameters</span></span>
<span data-ttu-id="07076-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="07076-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07076-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07076-121">Request headers</span></span>
|<span data-ttu-id="07076-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07076-122">Header</span></span>|<span data-ttu-id="07076-123">Valor</span><span class="sxs-lookup"><span data-stu-id="07076-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07076-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="07076-124">Authorization</span></span>|<span data-ttu-id="07076-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07076-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07076-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07076-126">Accept</span></span>|<span data-ttu-id="07076-127">application/json</span><span class="sxs-lookup"><span data-stu-id="07076-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07076-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07076-128">Request body</span></span>
<span data-ttu-id="07076-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="07076-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07076-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="07076-130">Response</span></span>
<span data-ttu-id="07076-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedEBook](../resources/intune-books-managedebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07076-131">If successful, this method returns a `200 OK` response code and [managedEBook](../resources/intune-books-managedebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07076-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07076-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="07076-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07076-133">Request</span></span>
<span data-ttu-id="07076-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07076-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="07076-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="07076-135">Response</span></span>
<span data-ttu-id="07076-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07076-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": {
    "@odata.type": "#microsoft.graph.managedEBook",
    "id": "1fbd3558-3558-1fbd-5835-bd1f5835bd1f",
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
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
  }
}
```









