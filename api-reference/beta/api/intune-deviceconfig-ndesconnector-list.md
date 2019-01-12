---
title: Lista ndesConnectors
description: Lista as propriedades e os relacionamentos dos objetos ndesConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c06fbaf735fbcdce0c0f1f9428d7c6bd75013450
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940516"
---
# <a name="list-ndesconnectors"></a><span data-ttu-id="abbb8-103">Lista ndesConnectors</span><span class="sxs-lookup"><span data-stu-id="abbb8-103">List ndesConnectors</span></span>

> <span data-ttu-id="abbb8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="abbb8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abbb8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="abbb8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abbb8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="abbb8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abbb8-107">Lista as propriedades e os relacionamentos dos objetos [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="abbb8-107">List properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="abbb8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abbb8-108">Prerequisites</span></span>
<span data-ttu-id="abbb8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abbb8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abbb8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abbb8-111">Permission type</span></span>|<span data-ttu-id="abbb8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="abbb8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abbb8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abbb8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abbb8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="abbb8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="abbb8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abbb8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abbb8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abbb8-116">Not supported.</span></span>|
|<span data-ttu-id="abbb8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abbb8-117">Application</span></span>|<span data-ttu-id="abbb8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abbb8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abbb8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abbb8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="abbb8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abbb8-120">Request headers</span></span>
|<span data-ttu-id="abbb8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abbb8-121">Header</span></span>|<span data-ttu-id="abbb8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="abbb8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abbb8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="abbb8-123">Authorization</span></span>|<span data-ttu-id="abbb8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abbb8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abbb8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abbb8-125">Accept</span></span>|<span data-ttu-id="abbb8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abbb8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abbb8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abbb8-127">Request body</span></span>
<span data-ttu-id="abbb8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="abbb8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abbb8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="abbb8-129">Response</span></span>
<span data-ttu-id="abbb8-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abbb8-130">If successful, this method returns a `200 OK` response code and a collection of [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abbb8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abbb8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="abbb8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abbb8-132">Request</span></span>
<span data-ttu-id="abbb8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abbb8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/ndesConnectors
```

### <a name="response"></a><span data-ttu-id="abbb8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="abbb8-134">Response</span></span>
<span data-ttu-id="abbb8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abbb8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ndesConnector",
      "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
      "state": "active",
      "displayName": "Display Name value"
    }
  ]
}
```





