---
title: Listar telecomExpenseManagementPartners
description: Lista propriedades e relações dos objetos telecomExpenseManagementPartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4689d12089bebe2b222d17ed4d4fe48016907191
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800309"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="93835-103">Listar telecomExpenseManagementPartners</span><span class="sxs-lookup"><span data-stu-id="93835-103">List telecomExpenseManagementPartners</span></span>

> <span data-ttu-id="93835-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="93835-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93835-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93835-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93835-106">Lista propriedades e relações dos objetos [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="93835-106">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93835-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="93835-107">Prerequisites</span></span>
<span data-ttu-id="93835-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93835-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93835-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93835-110">Permission type</span></span>|<span data-ttu-id="93835-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="93835-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93835-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93835-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93835-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="93835-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="93835-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93835-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93835-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93835-115">Not supported.</span></span>|
|<span data-ttu-id="93835-116">Application</span><span class="sxs-lookup"><span data-stu-id="93835-116">Application</span></span>|<span data-ttu-id="93835-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="93835-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93835-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93835-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="93835-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93835-119">Request headers</span></span>
|<span data-ttu-id="93835-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93835-120">Header</span></span>|<span data-ttu-id="93835-121">Valor</span><span class="sxs-lookup"><span data-stu-id="93835-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93835-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="93835-122">Authorization</span></span>|<span data-ttu-id="93835-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93835-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93835-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="93835-124">Accept</span></span>|<span data-ttu-id="93835-125">application/json</span><span class="sxs-lookup"><span data-stu-id="93835-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93835-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93835-126">Request body</span></span>
<span data-ttu-id="93835-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93835-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93835-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="93835-128">Response</span></span>
<span data-ttu-id="93835-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93835-129">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93835-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93835-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="93835-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93835-131">Request</span></span>
<span data-ttu-id="93835-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93835-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="93835-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="93835-133">Response</span></span>
<span data-ttu-id="93835-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93835-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




