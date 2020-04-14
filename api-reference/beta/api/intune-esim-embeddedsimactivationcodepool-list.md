---
title: Listar embeddedSIMActivationCodePools
description: Listar Propriedades e relações dos objetos embeddedSIMActivationCodePool.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e057333004a42b407f2dcd8752c43c43f035d27
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452212"
---
# <a name="list-embeddedsimactivationcodepools"></a><span data-ttu-id="f4c5d-103">Listar embeddedSIMActivationCodePools</span><span class="sxs-lookup"><span data-stu-id="f4c5d-103">List embeddedSIMActivationCodePools</span></span>

<span data-ttu-id="f4c5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4c5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4c5d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4c5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4c5d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4c5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4c5d-107">Listar Propriedades e relações dos objetos [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="f4c5d-107">List properties and relationships of the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4c5d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4c5d-108">Prerequisites</span></span>
<span data-ttu-id="f4c5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4c5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4c5d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4c5d-111">Permission type</span></span>|<span data-ttu-id="f4c5d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f4c5d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4c5d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4c5d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4c5d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4c5d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f4c5d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4c5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4c5d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4c5d-116">Not supported.</span></span>|
|<span data-ttu-id="f4c5d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4c5d-117">Application</span></span>|<span data-ttu-id="f4c5d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4c5d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4c5d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4c5d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="f4c5d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4c5d-120">Request headers</span></span>
|<span data-ttu-id="f4c5d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4c5d-121">Header</span></span>|<span data-ttu-id="f4c5d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f4c5d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4c5d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4c5d-123">Authorization</span></span>|<span data-ttu-id="f4c5d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4c5d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4c5d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4c5d-125">Accept</span></span>|<span data-ttu-id="f4c5d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4c5d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4c5d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4c5d-127">Request body</span></span>
<span data-ttu-id="f4c5d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f4c5d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4c5d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4c5d-129">Response</span></span>
<span data-ttu-id="f4c5d-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4c5d-130">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4c5d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4c5d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4c5d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4c5d-132">Request</span></span>
<span data-ttu-id="f4c5d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4c5d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
```

### <a name="response"></a><span data-ttu-id="f4c5d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4c5d-134">Response</span></span>
<span data-ttu-id="f4c5d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4c5d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 717

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
      "id": "ec308741-8741-ec30-4187-30ec418730ec",
      "displayName": "Display Name value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "activationCodes": [
        {
          "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
          "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
          "matchingIdentifier": "Matching Identifier value",
          "smdpPlusServerAddress": "Smdp Plus Server Address value"
        }
      ],
      "activationCodeCount": 3
    }
  ]
}
```



