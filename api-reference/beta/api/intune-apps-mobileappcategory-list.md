---
title: Listar mobileAppCategories
description: Listar propriedades e as relações dos objetos mobileAppCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bca59d6be158dc2f21d70765dea8d443dc0138b9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49248914"
---
# <a name="list-mobileappcategories"></a><span data-ttu-id="fef19-103">Listar mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="fef19-103">List mobileAppCategories</span></span>

<span data-ttu-id="fef19-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fef19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fef19-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fef19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fef19-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fef19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fef19-107">Listar propriedades e as relações dos objetos [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="fef19-107">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fef19-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fef19-108">Prerequisites</span></span>
<span data-ttu-id="fef19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fef19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fef19-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fef19-111">Permission type</span></span>|<span data-ttu-id="fef19-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fef19-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fef19-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fef19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fef19-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fef19-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fef19-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fef19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fef19-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fef19-116">Not supported.</span></span>|
|<span data-ttu-id="fef19-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fef19-117">Application</span></span>|<span data-ttu-id="fef19-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fef19-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fef19-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fef19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="fef19-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fef19-120">Request headers</span></span>
|<span data-ttu-id="fef19-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fef19-121">Header</span></span>|<span data-ttu-id="fef19-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fef19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fef19-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fef19-123">Authorization</span></span>|<span data-ttu-id="fef19-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fef19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fef19-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fef19-125">Accept</span></span>|<span data-ttu-id="fef19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fef19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fef19-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fef19-127">Request body</span></span>
<span data-ttu-id="fef19-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fef19-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fef19-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fef19-129">Response</span></span>
<span data-ttu-id="fef19-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fef19-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fef19-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fef19-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fef19-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fef19-132">Request</span></span>
<span data-ttu-id="fef19-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fef19-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
```

### <a name="response"></a><span data-ttu-id="fef19-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fef19-134">Response</span></span>
<span data-ttu-id="fef19-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fef19-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




