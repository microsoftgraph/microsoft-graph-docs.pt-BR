---
title: Listar mobileAppCategories
description: Listar propriedades e as relações dos objetos mobileAppCategory.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d6e411e2bc4e4bcb6c7f145a871a7bcb18e613e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394100"
---
# <a name="list-mobileappcategories"></a><span data-ttu-id="86cbd-103">Listar mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="86cbd-103">List mobileAppCategories</span></span>

> <span data-ttu-id="86cbd-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="86cbd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="86cbd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="86cbd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86cbd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="86cbd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86cbd-107">Listar propriedades e as relações dos objetos [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="86cbd-107">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86cbd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86cbd-108">Prerequisites</span></span>
<span data-ttu-id="86cbd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="86cbd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="86cbd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86cbd-111">Permission type</span></span>|<span data-ttu-id="86cbd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86cbd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86cbd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86cbd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86cbd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="86cbd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="86cbd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86cbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86cbd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86cbd-116">Not supported.</span></span>|
|<span data-ttu-id="86cbd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86cbd-117">Application</span></span>|<span data-ttu-id="86cbd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86cbd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86cbd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86cbd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="86cbd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86cbd-120">Request headers</span></span>
|<span data-ttu-id="86cbd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86cbd-121">Header</span></span>|<span data-ttu-id="86cbd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="86cbd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86cbd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="86cbd-123">Authorization</span></span>|<span data-ttu-id="86cbd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86cbd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86cbd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86cbd-125">Accept</span></span>|<span data-ttu-id="86cbd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86cbd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86cbd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86cbd-127">Request body</span></span>
<span data-ttu-id="86cbd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86cbd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86cbd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="86cbd-129">Response</span></span>
<span data-ttu-id="86cbd-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86cbd-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86cbd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86cbd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="86cbd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86cbd-132">Request</span></span>
<span data-ttu-id="86cbd-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86cbd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
```

### <a name="response"></a><span data-ttu-id="86cbd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="86cbd-134">Response</span></span>
<span data-ttu-id="86cbd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86cbd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




