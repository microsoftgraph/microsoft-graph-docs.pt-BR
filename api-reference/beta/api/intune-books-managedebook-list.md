---
title: Listar managedEBooks
description: Listar propriedades e relações dos objetos managedEBook.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ed8c5ef0d0e308a6fe241bc8b73516e69af3cc97
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392485"
---
# <a name="list-managedebooks"></a><span data-ttu-id="c7fbd-103">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="c7fbd-103">List managedEBooks</span></span>

<span data-ttu-id="c7fbd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7fbd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7fbd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7fbd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7fbd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7fbd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7fbd-107">Listar propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c7fbd-107">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7fbd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7fbd-108">Prerequisites</span></span>
<span data-ttu-id="c7fbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7fbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7fbd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7fbd-111">Permission type</span></span>|<span data-ttu-id="c7fbd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c7fbd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7fbd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7fbd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7fbd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7fbd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c7fbd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7fbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7fbd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7fbd-116">Not supported.</span></span>|
|<span data-ttu-id="c7fbd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7fbd-117">Application</span></span>|<span data-ttu-id="c7fbd-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7fbd-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7fbd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7fbd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="c7fbd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7fbd-120">Request headers</span></span>
|<span data-ttu-id="c7fbd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7fbd-121">Header</span></span>|<span data-ttu-id="c7fbd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c7fbd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7fbd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7fbd-123">Authorization</span></span>|<span data-ttu-id="c7fbd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7fbd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7fbd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7fbd-125">Accept</span></span>|<span data-ttu-id="c7fbd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7fbd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7fbd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7fbd-127">Request body</span></span>
<span data-ttu-id="c7fbd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7fbd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7fbd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7fbd-129">Response</span></span>
<span data-ttu-id="c7fbd-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedEBook](../resources/intune-books-managedebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7fbd-130">If successful, this method returns a `200 OK` response code and a collection of [managedEBook](../resources/intune-books-managedebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7fbd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7fbd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7fbd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7fbd-132">Request</span></span>
<span data-ttu-id="c7fbd-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7fbd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="c7fbd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7fbd-134">Response</span></span>
<span data-ttu-id="c7fbd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7fbd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



