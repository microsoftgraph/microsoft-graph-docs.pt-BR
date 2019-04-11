---
title: Listar dataSharingConsents
description: Listar Propriedades e relações dos objetos dataSharingConsent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b171ac3697a858e4cb8bfae3e030945fe07e7ae
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803133"
---
# <a name="list-datasharingconsents"></a><span data-ttu-id="baecb-103">Listar dataSharingConsents</span><span class="sxs-lookup"><span data-stu-id="baecb-103">List dataSharingConsents</span></span>

> <span data-ttu-id="baecb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="baecb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="baecb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="baecb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="baecb-106">Listar Propriedades e relações dos objetos [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="baecb-106">List properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="baecb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="baecb-107">Prerequisites</span></span>
<span data-ttu-id="baecb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baecb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baecb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="baecb-110">Permission type</span></span>|<span data-ttu-id="baecb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="baecb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="baecb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="baecb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="baecb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baecb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="baecb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="baecb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="baecb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="baecb-115">Not supported.</span></span>|
|<span data-ttu-id="baecb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="baecb-116">Application</span></span>|<span data-ttu-id="baecb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="baecb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="baecb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="baecb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="baecb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="baecb-119">Request headers</span></span>
|<span data-ttu-id="baecb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="baecb-120">Header</span></span>|<span data-ttu-id="baecb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="baecb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="baecb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="baecb-122">Authorization</span></span>|<span data-ttu-id="baecb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="baecb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="baecb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="baecb-124">Accept</span></span>|<span data-ttu-id="baecb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="baecb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="baecb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="baecb-126">Request body</span></span>
<span data-ttu-id="baecb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="baecb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="baecb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="baecb-128">Response</span></span>
<span data-ttu-id="baecb-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="baecb-129">If successful, this method returns a `200 OK` response code and a collection of [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baecb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="baecb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="baecb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="baecb-131">Request</span></span>
<span data-ttu-id="baecb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="baecb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents
```

### <a name="response"></a><span data-ttu-id="baecb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="baecb-133">Response</span></span>
<span data-ttu-id="baecb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="baecb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 447

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.dataSharingConsent",
      "id": "333387f7-87f7-3333-f787-3333f7873333",
      "serviceDisplayName": "Service Display Name value",
      "termsUrl": "https://example.com/termsUrl/",
      "granted": true,
      "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
      "grantedByUpn": "Granted By Upn value",
      "grantedByUserId": "Granted By User Id value"
    }
  ]
}
```





