---
title: Listar embeddedSIMActivationCodePools
description: Listar Propriedades e relações dos objetos embeddedSIMActivationCodePool.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f064b3dbf1f33060429b41fcc35ebca6b139538c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804923"
---
# <a name="list-embeddedsimactivationcodepools"></a><span data-ttu-id="81f51-103">Listar embeddedSIMActivationCodePools</span><span class="sxs-lookup"><span data-stu-id="81f51-103">List embeddedSIMActivationCodePools</span></span>

> <span data-ttu-id="81f51-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81f51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81f51-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81f51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81f51-106">Listar Propriedades e relações dos objetos [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="81f51-106">List properties and relationships of the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81f51-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81f51-107">Prerequisites</span></span>
<span data-ttu-id="81f51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81f51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81f51-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81f51-110">Permission type</span></span>|<span data-ttu-id="81f51-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81f51-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81f51-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81f51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81f51-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="81f51-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="81f51-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81f51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81f51-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81f51-115">Not supported.</span></span>|
|<span data-ttu-id="81f51-116">Application</span><span class="sxs-lookup"><span data-stu-id="81f51-116">Application</span></span>|<span data-ttu-id="81f51-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="81f51-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81f51-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81f51-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="81f51-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81f51-119">Request headers</span></span>
|<span data-ttu-id="81f51-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81f51-120">Header</span></span>|<span data-ttu-id="81f51-121">Valor</span><span class="sxs-lookup"><span data-stu-id="81f51-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81f51-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="81f51-122">Authorization</span></span>|<span data-ttu-id="81f51-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81f51-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81f51-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81f51-124">Accept</span></span>|<span data-ttu-id="81f51-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81f51-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81f51-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81f51-126">Request body</span></span>
<span data-ttu-id="81f51-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81f51-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81f51-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="81f51-128">Response</span></span>
<span data-ttu-id="81f51-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81f51-129">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81f51-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81f51-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="81f51-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81f51-131">Request</span></span>
<span data-ttu-id="81f51-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81f51-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
```

### <a name="response"></a><span data-ttu-id="81f51-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="81f51-133">Response</span></span>
<span data-ttu-id="81f51-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81f51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




