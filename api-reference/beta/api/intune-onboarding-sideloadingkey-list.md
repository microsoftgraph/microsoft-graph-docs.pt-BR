---
title: Listar sideLoadingKeies
description: Listar Propriedades e relações dos objetos sideLoadingKey.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1cda8acb55662ff9f13f416b3972d01fdf00e908
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972799"
---
# <a name="list-sideloadingkeies"></a><span data-ttu-id="f1021-103">Listar sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="f1021-103">List sideLoadingKeies</span></span>

> <span data-ttu-id="f1021-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f1021-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1021-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1021-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1021-106">Listar Propriedades e relações dos objetos [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="f1021-106">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1021-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1021-107">Prerequisites</span></span>
<span data-ttu-id="f1021-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1021-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1021-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1021-110">Permission type</span></span>|<span data-ttu-id="f1021-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1021-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1021-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1021-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1021-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1021-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f1021-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1021-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1021-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1021-115">Not supported.</span></span>|
|<span data-ttu-id="f1021-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1021-116">Application</span></span>|<span data-ttu-id="f1021-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1021-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1021-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1021-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="f1021-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1021-119">Request headers</span></span>
|<span data-ttu-id="f1021-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1021-120">Header</span></span>|<span data-ttu-id="f1021-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f1021-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1021-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1021-122">Authorization</span></span>|<span data-ttu-id="f1021-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1021-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1021-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1021-124">Accept</span></span>|<span data-ttu-id="f1021-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1021-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1021-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1021-126">Request body</span></span>
<span data-ttu-id="f1021-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1021-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1021-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1021-128">Response</span></span>
<span data-ttu-id="f1021-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1021-129">If successful, this method returns a `200 OK` response code and a collection of [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1021-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1021-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1021-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1021-131">Request</span></span>
<span data-ttu-id="f1021-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1021-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
```

### <a name="response"></a><span data-ttu-id="f1021-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1021-133">Response</span></span>
<span data-ttu-id="f1021-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1021-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sideLoadingKey",
      "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
      "value": "Value value",
      "displayName": "Display Name value",
      "description": "Description value",
      "totalActivation": 15,
      "lastUpdatedDateTime": "Last Updated Date Time value"
    }
  ]
}
```




