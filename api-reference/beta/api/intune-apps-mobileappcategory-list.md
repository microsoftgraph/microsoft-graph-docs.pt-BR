---
title: Listar mobileAppCategories
description: Listar propriedades e as relações dos objetos mobileAppCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 313bbf8341d45cd090d9b2fd3a98a7c950e556aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445026"
---
# <a name="list-mobileappcategories"></a><span data-ttu-id="bb5ce-103">Listar mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="bb5ce-103">List mobileAppCategories</span></span>

<span data-ttu-id="bb5ce-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bb5ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb5ce-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb5ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb5ce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb5ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb5ce-107">Listar propriedades e as relações dos objetos [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="bb5ce-107">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb5ce-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb5ce-108">Prerequisites</span></span>
<span data-ttu-id="bb5ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb5ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb5ce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb5ce-111">Permission type</span></span>|<span data-ttu-id="bb5ce-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb5ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb5ce-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb5ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb5ce-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb5ce-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bb5ce-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb5ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb5ce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb5ce-116">Not supported.</span></span>|
|<span data-ttu-id="bb5ce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb5ce-117">Application</span></span>|<span data-ttu-id="bb5ce-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb5ce-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb5ce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb5ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="bb5ce-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb5ce-120">Request headers</span></span>
|<span data-ttu-id="bb5ce-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb5ce-121">Header</span></span>|<span data-ttu-id="bb5ce-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bb5ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb5ce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb5ce-123">Authorization</span></span>|<span data-ttu-id="bb5ce-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb5ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb5ce-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb5ce-125">Accept</span></span>|<span data-ttu-id="bb5ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb5ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb5ce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb5ce-127">Request body</span></span>
<span data-ttu-id="bb5ce-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb5ce-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb5ce-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb5ce-129">Response</span></span>
<span data-ttu-id="bb5ce-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb5ce-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb5ce-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb5ce-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb5ce-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb5ce-132">Request</span></span>
<span data-ttu-id="bb5ce-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb5ce-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
```

### <a name="response"></a><span data-ttu-id="bb5ce-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb5ce-134">Response</span></span>
<span data-ttu-id="bb5ce-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb5ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppCategory",
      "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```





