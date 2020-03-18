---
title: Listar managedEBookCategories
description: Listar Propriedades e relações dos objetos managedEBookCategory.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 218a5a87c3e2291c1bf28be81482fa162e192f4c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760358"
---
# <a name="list-managedebookcategories"></a><span data-ttu-id="c6fbe-103">Listar managedEBookCategories</span><span class="sxs-lookup"><span data-stu-id="c6fbe-103">List managedEBookCategories</span></span>

> <span data-ttu-id="c6fbe-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c6fbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6fbe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6fbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6fbe-106">Listar Propriedades e relações dos objetos [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="c6fbe-106">List properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6fbe-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c6fbe-107">Prerequisites</span></span>
<span data-ttu-id="c6fbe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6fbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6fbe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6fbe-110">Permission type</span></span>|<span data-ttu-id="c6fbe-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c6fbe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6fbe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6fbe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6fbe-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6fbe-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c6fbe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6fbe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6fbe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6fbe-115">Not supported.</span></span>|
|<span data-ttu-id="c6fbe-116">Application</span><span class="sxs-lookup"><span data-stu-id="c6fbe-116">Application</span></span>|<span data-ttu-id="c6fbe-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6fbe-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6fbe-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6fbe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBookCategories
GET /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="c6fbe-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6fbe-119">Request headers</span></span>
|<span data-ttu-id="c6fbe-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6fbe-120">Header</span></span>|<span data-ttu-id="c6fbe-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c6fbe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6fbe-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6fbe-122">Authorization</span></span>|<span data-ttu-id="c6fbe-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6fbe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6fbe-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c6fbe-124">Accept</span></span>|<span data-ttu-id="c6fbe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6fbe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6fbe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6fbe-126">Request body</span></span>
<span data-ttu-id="c6fbe-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c6fbe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6fbe-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6fbe-128">Response</span></span>
<span data-ttu-id="c6fbe-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [managedEBookCategory](../resources/intune-books-managedebookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6fbe-129">If successful, this method returns a `200 OK` response code and a collection of [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6fbe-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6fbe-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6fbe-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6fbe-131">Request</span></span>
<span data-ttu-id="c6fbe-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6fbe-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
```

### <a name="response"></a><span data-ttu-id="c6fbe-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6fbe-133">Response</span></span>
<span data-ttu-id="c6fbe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6fbe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 264

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBookCategory",
      "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




