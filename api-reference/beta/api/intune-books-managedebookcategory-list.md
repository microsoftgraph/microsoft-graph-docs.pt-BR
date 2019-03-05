---
title: Listar managedEBookCategories
description: Listar Propriedades e relações dos objetos managedEBookCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b67f1c02fb0d7aa141c6889e92b3238baa6a4a5a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152497"
---
# <a name="list-managedebookcategories"></a><span data-ttu-id="67a39-103">Listar managedEBookCategories</span><span class="sxs-lookup"><span data-stu-id="67a39-103">List managedEBookCategories</span></span>

> <span data-ttu-id="67a39-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67a39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67a39-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67a39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67a39-106">Listar Propriedades e relações dos objetos [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="67a39-106">List properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67a39-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67a39-107">Prerequisites</span></span>
<span data-ttu-id="67a39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="67a39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="67a39-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67a39-110">Permission type</span></span>|<span data-ttu-id="67a39-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67a39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67a39-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67a39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67a39-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="67a39-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="67a39-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67a39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67a39-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67a39-115">Not supported.</span></span>|
|<span data-ttu-id="67a39-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67a39-116">Application</span></span>|<span data-ttu-id="67a39-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67a39-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67a39-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67a39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBookCategories
GET /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="67a39-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67a39-119">Request headers</span></span>
|<span data-ttu-id="67a39-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67a39-120">Header</span></span>|<span data-ttu-id="67a39-121">Valor</span><span class="sxs-lookup"><span data-stu-id="67a39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67a39-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="67a39-122">Authorization</span></span>|<span data-ttu-id="67a39-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67a39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67a39-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67a39-124">Accept</span></span>|<span data-ttu-id="67a39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67a39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67a39-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67a39-126">Request body</span></span>
<span data-ttu-id="67a39-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67a39-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67a39-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a39-128">Response</span></span>
<span data-ttu-id="67a39-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [managedEBookCategory](../resources/intune-books-managedebookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67a39-129">If successful, this method returns a `200 OK` response code and a collection of [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67a39-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67a39-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="67a39-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67a39-131">Request</span></span>
<span data-ttu-id="67a39-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67a39-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
```

### <a name="response"></a><span data-ttu-id="67a39-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a39-133">Response</span></span>
<span data-ttu-id="67a39-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67a39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




