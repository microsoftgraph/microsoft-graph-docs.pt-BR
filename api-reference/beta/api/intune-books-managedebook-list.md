---
title: Listar managedEBooks
description: Listar propriedades e relações dos objetos managedEBook.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 349173110e1276d7400dd23dc12cc84c4f675ad9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328393"
---
# <a name="list-managedebooks"></a><span data-ttu-id="6da27-103">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="6da27-103">List managedEBooks</span></span>

> <span data-ttu-id="6da27-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6da27-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6da27-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6da27-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6da27-106">Listar propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="6da27-106">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6da27-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6da27-107">Prerequisites</span></span>
<span data-ttu-id="6da27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6da27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6da27-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6da27-110">Permission type</span></span>|<span data-ttu-id="6da27-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6da27-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6da27-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6da27-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6da27-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6da27-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6da27-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6da27-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6da27-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6da27-115">Not supported.</span></span>|
|<span data-ttu-id="6da27-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6da27-116">Application</span></span>|<span data-ttu-id="6da27-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6da27-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6da27-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6da27-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="6da27-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6da27-119">Request headers</span></span>
|<span data-ttu-id="6da27-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6da27-120">Header</span></span>|<span data-ttu-id="6da27-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6da27-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6da27-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6da27-122">Authorization</span></span>|<span data-ttu-id="6da27-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6da27-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6da27-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6da27-124">Accept</span></span>|<span data-ttu-id="6da27-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6da27-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6da27-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6da27-126">Request body</span></span>
<span data-ttu-id="6da27-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6da27-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6da27-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6da27-128">Response</span></span>
<span data-ttu-id="6da27-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedEBook](../resources/intune-books-managedebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6da27-129">If successful, this method returns a `200 OK` response code and a collection of [managedEBook](../resources/intune-books-managedebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6da27-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6da27-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6da27-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6da27-131">Request</span></span>
<span data-ttu-id="6da27-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6da27-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="6da27-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6da27-133">Response</span></span>
<span data-ttu-id="6da27-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6da27-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": [
    {
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
  ]
}
```






