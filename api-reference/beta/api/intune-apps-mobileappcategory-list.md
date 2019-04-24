---
title: Listar mobileAppCategories
description: Listar propriedades e as relações dos objetos mobileAppCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cecb7649d3b1d08de6f1f945b355516ac79d5c3e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32489286"
---
# <a name="list-mobileappcategories"></a><span data-ttu-id="26a09-103">Listar mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="26a09-103">List mobileAppCategories</span></span>

> <span data-ttu-id="26a09-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26a09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26a09-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26a09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26a09-106">Listar propriedades e as relações dos objetos [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="26a09-106">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26a09-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26a09-107">Prerequisites</span></span>
<span data-ttu-id="26a09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26a09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26a09-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26a09-110">Permission type</span></span>|<span data-ttu-id="26a09-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="26a09-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26a09-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26a09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26a09-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="26a09-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="26a09-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26a09-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26a09-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26a09-115">Not supported.</span></span>|
|<span data-ttu-id="26a09-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26a09-116">Application</span></span>|<span data-ttu-id="26a09-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26a09-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26a09-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26a09-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="26a09-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26a09-119">Request headers</span></span>
|<span data-ttu-id="26a09-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26a09-120">Header</span></span>|<span data-ttu-id="26a09-121">Valor</span><span class="sxs-lookup"><span data-stu-id="26a09-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26a09-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="26a09-122">Authorization</span></span>|<span data-ttu-id="26a09-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26a09-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26a09-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26a09-124">Accept</span></span>|<span data-ttu-id="26a09-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26a09-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26a09-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26a09-126">Request body</span></span>
<span data-ttu-id="26a09-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="26a09-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26a09-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="26a09-128">Response</span></span>
<span data-ttu-id="26a09-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26a09-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26a09-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26a09-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="26a09-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26a09-131">Request</span></span>
<span data-ttu-id="26a09-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26a09-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
```

### <a name="response"></a><span data-ttu-id="26a09-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="26a09-133">Response</span></span>
<span data-ttu-id="26a09-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26a09-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





