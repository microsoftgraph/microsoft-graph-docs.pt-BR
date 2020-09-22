---
title: Listar telecomExpenseManagementPartners
description: Lista propriedades e relações dos objetos telecomExpenseManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b9cf187a68ca3350884279fb2569f890deec41c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082179"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="90867-103">Listar telecomExpenseManagementPartners</span><span class="sxs-lookup"><span data-stu-id="90867-103">List telecomExpenseManagementPartners</span></span>

<span data-ttu-id="90867-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90867-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90867-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="90867-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90867-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90867-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90867-107">Lista propriedades e relações dos objetos [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="90867-107">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90867-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90867-108">Prerequisites</span></span>
<span data-ttu-id="90867-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90867-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90867-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90867-111">Permission type</span></span>|<span data-ttu-id="90867-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90867-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90867-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90867-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90867-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="90867-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="90867-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90867-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90867-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90867-116">Not supported.</span></span>|
|<span data-ttu-id="90867-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90867-117">Application</span></span>|<span data-ttu-id="90867-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="90867-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90867-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90867-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="90867-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90867-120">Request headers</span></span>
|<span data-ttu-id="90867-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90867-121">Header</span></span>|<span data-ttu-id="90867-122">Valor</span><span class="sxs-lookup"><span data-stu-id="90867-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90867-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="90867-123">Authorization</span></span>|<span data-ttu-id="90867-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90867-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90867-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90867-125">Accept</span></span>|<span data-ttu-id="90867-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90867-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90867-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90867-127">Request body</span></span>
<span data-ttu-id="90867-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90867-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90867-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="90867-129">Response</span></span>
<span data-ttu-id="90867-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90867-130">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90867-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90867-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="90867-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90867-132">Request</span></span>
<span data-ttu-id="90867-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90867-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="90867-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="90867-134">Response</span></span>
<span data-ttu-id="90867-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90867-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






