---
title: Listar dataSharingConsents
description: Listar Propriedades e relações dos objetos dataSharingConsent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ab72e31caac71f09d5e74e74500f460b738516a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959205"
---
# <a name="list-datasharingconsents"></a><span data-ttu-id="48513-103">Listar dataSharingConsents</span><span class="sxs-lookup"><span data-stu-id="48513-103">List dataSharingConsents</span></span>

> <span data-ttu-id="48513-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48513-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48513-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48513-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48513-106">Listar Propriedades e relações dos objetos [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="48513-106">List properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48513-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="48513-107">Prerequisites</span></span>
<span data-ttu-id="48513-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48513-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48513-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48513-110">Permission type</span></span>|<span data-ttu-id="48513-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="48513-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48513-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48513-112">Delegated (work or school account)</span></span>|<span data-ttu-id="48513-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48513-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="48513-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48513-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48513-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48513-115">Not supported.</span></span>|
|<span data-ttu-id="48513-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48513-116">Application</span></span>|<span data-ttu-id="48513-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48513-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48513-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48513-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="48513-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48513-119">Request headers</span></span>
|<span data-ttu-id="48513-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48513-120">Header</span></span>|<span data-ttu-id="48513-121">Valor</span><span class="sxs-lookup"><span data-stu-id="48513-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48513-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="48513-122">Authorization</span></span>|<span data-ttu-id="48513-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48513-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48513-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="48513-124">Accept</span></span>|<span data-ttu-id="48513-125">application/json</span><span class="sxs-lookup"><span data-stu-id="48513-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48513-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48513-126">Request body</span></span>
<span data-ttu-id="48513-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="48513-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48513-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="48513-128">Response</span></span>
<span data-ttu-id="48513-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48513-129">If successful, this method returns a `200 OK` response code and a collection of [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48513-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48513-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="48513-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48513-131">Request</span></span>
<span data-ttu-id="48513-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48513-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents
```

### <a name="response"></a><span data-ttu-id="48513-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="48513-133">Response</span></span>
<span data-ttu-id="48513-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48513-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





