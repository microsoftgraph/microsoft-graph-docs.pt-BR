---
title: Listar telecomExpenseManagementPartners
description: Lista propriedades e relações dos objetos telecomExpenseManagementPartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b295168ef2d128a284a63ad0513c9b281197805
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511912"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="e1ee6-103">Listar telecomExpenseManagementPartners</span><span class="sxs-lookup"><span data-stu-id="e1ee6-103">List telecomExpenseManagementPartners</span></span>

<span data-ttu-id="e1ee6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1ee6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1ee6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1ee6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1ee6-106">Lista propriedades e relações dos objetos [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="e1ee6-106">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1ee6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1ee6-107">Prerequisites</span></span>
<span data-ttu-id="e1ee6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1ee6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1ee6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1ee6-110">Permission type</span></span>|<span data-ttu-id="e1ee6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1ee6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1ee6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1ee6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1ee6-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1ee6-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e1ee6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1ee6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1ee6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1ee6-115">Not supported.</span></span>|
|<span data-ttu-id="e1ee6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1ee6-116">Application</span></span>|<span data-ttu-id="e1ee6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1ee6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1ee6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1ee6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="e1ee6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1ee6-119">Request headers</span></span>
|<span data-ttu-id="e1ee6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1ee6-120">Header</span></span>|<span data-ttu-id="e1ee6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e1ee6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1ee6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1ee6-122">Authorization</span></span>|<span data-ttu-id="e1ee6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1ee6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1ee6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1ee6-124">Accept</span></span>|<span data-ttu-id="e1ee6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e1ee6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1ee6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1ee6-126">Request body</span></span>
<span data-ttu-id="e1ee6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1ee6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1ee6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1ee6-128">Response</span></span>
<span data-ttu-id="e1ee6-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1ee6-129">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1ee6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1ee6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1ee6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1ee6-131">Request</span></span>
<span data-ttu-id="e1ee6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1ee6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="e1ee6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1ee6-133">Response</span></span>
<span data-ttu-id="e1ee6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1ee6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




