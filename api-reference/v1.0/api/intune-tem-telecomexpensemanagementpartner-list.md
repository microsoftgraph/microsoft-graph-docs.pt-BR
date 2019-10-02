---
title: Listar telecomExpenseManagementPartners
description: Lista propriedades e relações dos objetos telecomExpenseManagementPartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0ee23a4ee886c01f060ac48353fe597730764c9d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361161"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="e9393-103">Listar telecomExpenseManagementPartners</span><span class="sxs-lookup"><span data-stu-id="e9393-103">List telecomExpenseManagementPartners</span></span>

> <span data-ttu-id="e9393-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9393-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9393-105">Lista propriedades e relações dos objetos [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="e9393-105">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9393-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9393-106">Prerequisites</span></span>
<span data-ttu-id="e9393-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9393-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9393-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9393-109">Permission type</span></span>|<span data-ttu-id="e9393-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e9393-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9393-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9393-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e9393-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9393-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e9393-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9393-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9393-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9393-114">Not supported.</span></span>|
|<span data-ttu-id="e9393-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9393-115">Application</span></span>|<span data-ttu-id="e9393-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9393-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9393-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9393-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="e9393-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9393-118">Request headers</span></span>
|<span data-ttu-id="e9393-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9393-119">Header</span></span>|<span data-ttu-id="e9393-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e9393-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9393-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9393-121">Authorization</span></span>|<span data-ttu-id="e9393-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9393-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9393-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9393-123">Accept</span></span>|<span data-ttu-id="e9393-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e9393-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9393-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9393-125">Request body</span></span>
<span data-ttu-id="e9393-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9393-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9393-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9393-127">Response</span></span>
<span data-ttu-id="e9393-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9393-128">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9393-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9393-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9393-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9393-130">Request</span></span>
<span data-ttu-id="e9393-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9393-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="e9393-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9393-132">Response</span></span>
<span data-ttu-id="e9393-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9393-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 358

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
      "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
      "displayName": "Display Name value",
      "url": "Url value",
      "appAuthorized": true,
      "enabled": true,
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
    }
  ]
}
```




